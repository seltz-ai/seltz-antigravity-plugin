---
name: seltz-web-search
description: DEFAULT for all web search and research queries. Use when the user needs current information, news, company or people research, documentation, fact-checking, or any question requiring live web data.
---

# Web Search (Seltz)

Use the Seltz `search` tool for any question that needs current or external information: news, company or people research, documentation, fact-checking.

## Parameters

- `query` (required): concise keywords
- `scope` (optional): `news`, `companies`, `people`, `financial-reports` or `wikipedia`. Omit it for general queries.
- `from_date` / `to_date` (optional, YYYY-MM-DD): for recent or dated news. Not with the `companies` or `people` scopes.
- `include_domains` / `exclude_domains` (optional): restrict or exclude sources
- `max_results` (optional, default 10)

## Tips

- For broad topics, run several focused queries in parallel
- For people, add a company or role, since a bare name returns several candidates
- If a result's content is not enough, call `fetch` on its URL

## Output

Lead with the direct answer and cite every fact with its source URL.

## If Seltz is not connected

Tell the user to check that the Seltz plugin is enabled and that their API key from https://console.seltz.ai is set.
