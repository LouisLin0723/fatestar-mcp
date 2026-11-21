# FateStar MCP — Zi Wei Dou Shu (紫微斗数) for AI agents

Remote MCP server for Zi Wei Dou Shu (Purple Star Astrology): cast birth charts, read decade/annual transits,
and ask the AI reader "Zheng Daqian" (郑大钱) questions about a chart.

- Endpoint (OAuth): https://www.fatestar.top/mcp
- Endpoint (API key header): https://www.fatestar.top/api/mcp
- School: San He (三合派). Geng-stem Si Hua: Lu Tai Yang, Quan Wu Qu, Ke Tian Tong, Ji Tai Yin.
- Pricing: charts and transits are free; AI readings cost US$0.10 (long questions US$0.20). New accounts get a one-time US$3 trial.

## Tools

| Tool | What it does | Cost |
|---|---|---|
| ziwei_chart | Natal chart: 12 palaces, 14 main stars, brightness, Si Hua, patterns | Free |
| ziwei_transits | Decade / minor / annual / monthly / daily / hourly periods | Free |
| ziwei_reading | AI reading of a chart for a question | Paid |
| fatestar_credits | Remaining credits | Free (sign-in) |
| fatestar_list_charts / fatestar_get_chart / fatestar_save_chart | Charts saved in your account | Free (sign-in) |

## Install

Claude Code:
    claude mcp add --transport http --scope user fatestar https://www.fatestar.top/mcp

Codex:
    codex mcp add fatestar --url https://www.fatestar.top/mcp && codex mcp login fatestar

Cursor (~/.cursor/mcp.json):
    { "mcpServers": { "fatestar": { "url": "https://www.fatestar.top/mcp" } } }

Claude Desktop / claude.ai: Settings → Connectors → Add custom connector → https://www.fatestar.top/mcp

Full guide for agents: https://www.fatestar.top/agent.md

## Learn Zi Wei Dou Shu
- The 14 Main Stars: https://www.fatestar.top/ziwei-doushu/learn/14-main-stars
- The 12 Palaces: https://www.fatestar.top/ziwei-doushu/learn/12-palaces
- The Four Transformations: https://www.fatestar.top/ziwei-doushu/learn/four-transformations
- San He vs Fei Xing: https://www.fatestar.top/ziwei-doushu/learn/san-he-vs-fei-xing

Listed in the official MCP Registry as `top.fatestar/zwds` (see [server.json](server.json)).

Readings are cultural and reflective, not medical, legal, mental-health or financial advice.
