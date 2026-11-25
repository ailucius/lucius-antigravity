# Lucius AI for Antigravity

Lucius AI finds open public tenders and reads tender packs. This plugin adds the Lucius MCP server to Antigravity, so the agent can search notices and read an analysed pack while you work.

## What it adds

One remote MCP server, `lucius`, at https://api.ailucius.com/api/v1/mcp, with six tools:

- `search_tenders`: searches open public tenders by words, country, source, CPV prefix and closing date.
- `get_tender`: reads one notice: its metadata, a snippet, the documents and links its source lists, and your workspace's own stored analysis when it has one.
- `similar_tenders`: finds notices similar to a given one.
- `ask_market`: answers a market question in plain words over the public index of notices and award records, and returns the SQL that ran with its result table.
- `analyze_pack`: starts the analysis of a tender pack, from a public link or from the tender_id of a notice found with search_tenders. Each analysis uses one of the workspace's monthly analyses.
- `get_pack_analysis`: reads the analysis: the bid call, the requirements with their quotes and pages, which of them decide the bid, and the forms to return.

## Sign in

The first time the agent calls a Lucius tool, Antigravity opens the Lucius sign-in page. Sign in with your Lucius account and approve the access. Starting an analysis uses one of your workspace's monthly analyses, and what an analysis includes depends on your Lucius plan.

## Data

Notices come from public procurement sources. A pack you analyse stays in your Lucius workspace. Details: https://ailucius.com/trust

## Support

contact@ailucius.com
