---
name: seltz-fetch
description: Read the full content of web pages as clean markdown using Seltz. Use when the user shares a URL or a search result needs more detail. Use seltz-web-search instead when you need to find pages first.
---

# Fetch URL (Seltz)

Use the Seltz `fetch` tool to read the full content of web pages as markdown.

## Parameters

- `urls` (required): 1 to 5 http or https URLs per call.

## Notes

- Each URL gets its own result: match results on `requested_url`. One failing URL does not affect the others.
- HTML pages only: PDFs and images are rejected.

## Output

Answer the user's question from the page content and include the source URL.

## If Seltz is not connected

Tell the user to check that the Seltz plugin is enabled and that their API key from https://console.seltz.ai is set.
