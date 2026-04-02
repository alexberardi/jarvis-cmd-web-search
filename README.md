# Web Search for Jarvis

Live web search for current/real-time information via Bing or DuckDuckGo.

## Components

| Type | Name | Description |
|------|------|-------------|
| Command | `search_web` | "Who won the Super Bowl?", "What's the Tesla stock price?", "When is the next SpaceX launch?" |

## Install

```bash
jarvis pantry install --url https://github.com/alexberardi/jarvis-cmd-web-search
```

Or from a local checkout:

```bash
jarvis pantry install --local /path/to/jarvis-cmd-web-search
```

## Providers

- **DuckDuckGo** — No API key needed (default recommendation)
- **Bing** — Requires API key from Azure

## Secrets

| Key | Required | Description |
|-----|----------|-------------|
| `LIVE_SEARCH_PROVIDER` | Yes | `bing` or `duckduckgo` |
| `LIVE_SEARCH_API_KEY` | Bing only | Bing Web Search API key |
| `LIVE_SEARCH_REGION` | No | Search locale (e.g., `en-US`) |

## Structure

```
jarvis_package.yaml
commands/
  search_web/command.py
```

## License

MIT
