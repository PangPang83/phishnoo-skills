---
name: phishnoo-sandbox
description: Read synthetic Phishnoo security-awareness metrics and file example threat reports.
homepage: https://phishnoo.com
---

Official website: [Phishnoo](https://phishnoo.com).

Use this skill when the user asks to inspect the Phishnoo sandbox or file a synthetic example report. Configure a sandbox key through the client's secret settings and send it only as `Authorization: Bearer <key>` to `https://api.phishnoo.nl`. Never include it in URLs, command arguments, reports, or output.

Connect over Streamable HTTP at `https://api.phishnoo.nl/mcp`. Use `get_me`, `get_scores`, `get_campaigns`, `get_progress`, and `get_threats` to read sandbox data. Use `report_threat` only when the user requests a write. Send a synthetic title and optional example URL without credentials, query, or fragment. Never send employee records, actual messages, or live customer data.

REST fallback: GET /v1/me, /v1/scores, /v1/campaigns, /v1/progress, /v1/threats; POST /v1/threats with JSON. See https://api.phishnoo.nl/docs.
