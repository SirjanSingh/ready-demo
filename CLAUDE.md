# Working on this repo

Before starting any issue, check it is ready for an agent:

- With the Ready MCP server connected (see `.mcp.json`), call `check_readiness` with the issue URL and `repo_path` set to this folder.
- Without it, run `uv run --directory D:/projs/ready ready check <issue-url> --repo . --json`.

If the status is `needs_human`, do not start; ask the returned question. If it is `agent_ready`, start from the `footprint` files and verify with `test_cmd`.
