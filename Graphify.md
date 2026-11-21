# SETUP.md

One-time setup for Graphify, then work graph-first.

`graphify` turns this repo into a queryable knowledge graph (AST, local, no LLM needed for code).
An agent then answers codebase questions by querying the graph instead of grepping files.

## Master prompt

Paste everything inside the block below into your AI assistant (Kilo, Claude Code, Codex, Cursor)
with the project root as the working directory.

````text
You are setting up Graphify for this repository, then switching to graph-first work.

Source of truth: https://github.com/Graphify-Labs/graphify
Official PyPI package: `graphifyy` (double-y). The CLI command is `graphify`.

Scope rules:
- Work only inside this repository.
- Do not modify source code, do not commit, do not push.
- Do not delete or overwrite existing content in AGENTS.md.

Phase 1 - Install the CLI
1. Run `graphify --version`. If it works, skip to Phase 2.
2. If it fails, install it. Prefer, in order:
   - `uv tool install graphifyy` (recommended, isolated env; on Windows the binary lands in
     %USERPROFILE%\.local\bin, which must be on PATH)
   - `pipx install graphifyy`
   - `python -m pip install graphifyy`
   Requirements: Python 3.11.5 to 3.14. If `uv` is missing: `winget install astral-sh.uv`
   on Windows, `brew install uv` on macOS, `curl -LsSf https://astral.sh/uv/install.sh | sh`
   on Linux.
3. If this repo contains .sql files, install the SQL parser too:
   `uv tool install "graphifyy[sql]" --force`. Without it, SQL files contribute zero nodes.
4. Verify with `graphify --version`. Report the version.

Phase 2 - Wire the assistant into AGENTS.md
1. Detect which assistant is running, then run the matching installer:
   - Kilo Code:        `graphify kilo install`
   - Claude Code:      `graphify install`
   - Codex:            `graphify install --platform codex`
   - OpenCode:         `graphify install --platform opencode`
   - Cursor:           `graphify cursor install`
   - Gemini CLI:       `graphify install --platform gemini`
   - GitHub Copilot:   `graphify install --platform copilot`
   - Agent Skills:     `graphify install --platform agents`
   Run `graphify install --help` for the full platform list.
2. AGENTS.md handling, do this by hand if the installer did not do it:
   - If AGENTS.md does not exist: create it containing only the graphify section below.
   - If AGENTS.md already exists: APPEND the graphify section at the end. Never rewrite,
     reorder, or truncate the existing content. Do not merge it into an existing section.
   - The section heading must be exactly `## graphify` on its own line, at column 0, so a
     later `graphify kilo install` run can find and update it in place instead of appending
     a duplicate.
   - The section body is the "Always-on rules" block in Phase 4 below.
3. Verify the result: the file must contain exactly one `## graphify` heading, and every line
   that existed before your edit must still be present. Report both facts.

Phase 3 - Build the graph
1. If `graphify-out/graph.json` already exists, skip to Phase 4 and run `graphify update .`
   instead of a full rebuild.
2. Build it. Preferred path: invoke the `/graphify` skill with the project root as target
   (Kilo: `/graphify .`). That runs the full pipeline and labels the communities.
   Headless fallback, no API key needed, code only:
     graphify extract . --code-only
     graphify cluster-only . --no-label
   To include docs, papers and images you need a semantic pass. It uses the host assistant
   itself when no Gemini key is set, or `GEMINI_API_KEY` / `GOOGLE_API_KEY` when one is.
   Never ask the user for an Anthropic or OpenAI key; graphify does not read those.
3. Expected output in `graphify-out/`:
   - `graph.json`      the graph data, queried by the CLI
   - `GRAPH_REPORT.md` god nodes, communities, surprising connections
   - `graph.html`      interactive graph, open in a browser
4. Add `graphify-out/` to `.gitignore` unless the team explicitly wants to commit the graph.
   A committed `graph.json` is rewritten whole on every build, so a large diff is expected.
5. Report: node count, edge count, community count, and the top 5 god nodes.

Phase 4 - Always-on rules (this is the AGENTS.md section body)
```markdown
## graphify

This project has a knowledge graph at graphify-out/ with god nodes, community structure, and cross-file relationships.

When the user types `/graphify`, use the installed graphify skill or instructions before doing anything else.

Rules:
- When graphify-out/graph.json exists, run `graphify query "<question>"` before your first grep, search or source-file read for a codebase question, and put this rule in every subagent prompt that explores code. Read raw files only for lines the graph or an earlier read already located. Use `graphify path "<A>" "<B>"` for relationships and `graphify explain "<concept>"` for focused concepts. When the answer is under a Markdown heading, `graphify section "<heading>"` prints that section's text, so the .md need not be opened. These return a scoped subgraph, usually much smaller than GRAPH_REPORT.md or raw grep output.
- Dirty graphify-out/ files are expected after hooks or incremental updates; dirty graph files are not a reason to skip graphify. Only skip graphify if the task is about stale or incorrect graph output, or the user explicitly says not to use it.
- If graphify-out/wiki/index.md exists, use it for broad navigation instead of raw source browsing.
- Read graphify-out/GRAPH_REPORT.md only for broad architecture review or when query/path/explain do not surface enough context.
- After modifying code, run `graphify update .` to keep the graph current (AST-only, no API cost).
- A committed graphify-out/graph.json is rewritten whole on every build, so a large diff to it in a pull request is expected. Do not flag it as churn or suggest skipping the graph rebuild or its hooks.
```

Phase 5 - Confirm and hand back
1. Prove the graph answers a question about this repo:
   `graphify query "<a real question about this codebase>"`
2. Prove the path tool works: `graphify path "<symbol A>" "<symbol B>"`
3. Print the final state: graphify version, graph location, node/edge/community counts,
   whether AGENTS.md was created or appended to, and the top 5 god nodes.
4. State clearly that from now on you will query the graph before searching files, and that
   you will run `graphify update .` after changing code.
````

## What the master prompt does, step by step

| Phase | Action | Artifact |
|---|---|---|
| 1 | Install the `graphify` CLI (`uv tool install graphifyy`) | binary on PATH |
| 2 | Run the installer for your assistant, then write or append `AGENTS.md` | `## graphify` section |
| 3 | Build the graph (`/graphify .`) | `graphify-out/` |
| 4 | Paste the always-on rules into `AGENTS.md` | rules that survive future sessions |
| 5 | Verify with a real query | proof it works |

## AGENTS.md rules

The installer writes the `## graphify` section into `AGENTS.md` itself. It replaces that section
in place on every re-run, so the file never grows duplicate blocks, and it never touches the
rest of your file.

If you prefer to manage the section by hand, keep the heading exactly `## graphify` at column 0.
Any other heading text means a later installer run will append a second copy instead of updating
the first.

## After setup

The graph goes stale as the code changes. Run this after editing code:

```bash
graphify update .
```

It re-extracts only changed files, uses AST only, and costs no LLM tokens.

Useful commands:

```bash
graphify query "<question>"        # scoped subgraph for a question
graphify path "<A>" "<B>"          # how two things connect
graphify explain "<symbol>"        # one concept and its neighbors
graphify section "<Heading>"       # print one Markdown section
graphify god-nodes --top 10        # architectural hubs
graphify affected "<symbol>"       # reverse traversal, blast radius
graphify benchmark                 # token reduction vs naive reading
graphify check-update .            # is a rebuild pending
```

## Troubleshooting

`graphify: command not found`
The binary is in `%USERPROFILE%\.local\bin` on Windows. Add it to PATH, then reopen the shell.

`tree_sitter_sql not installed`
SQL files contribute nothing to the graph. Run `uv tool install "graphifyy[sql]" --force`, then
`graphify update .`.

Graph looks populated but real symbols are missing
An ambiguous extension was parsed as the wrong language. Declare it in the repo, for example
`.graphifyrc` with a per-extension language override, then rebuild with `--force`.

Semantic pass asks for a key
Only `GEMINI_API_KEY` or `GOOGLE_API_KEY` are read. Without them, the host assistant does the
semantic extraction itself.
