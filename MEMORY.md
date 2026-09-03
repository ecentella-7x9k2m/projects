# Persistent Memory — Human Reference

_This file mirrors the content of my persistent `memory` tool (2,200 char limit). Updated for reference._

## Astralplex Stack
- Jellyfin (8096), Sonarr v4 (8989), Prowlarr (9696), Jackett (9117 localhost), FlareSolverr (8191)
- qBittorrent on 192.168.50.x via ProtonVPN tunnel — dynamic WebUI port, Sonarr→qB at 192.168.50.79:{port}
- DHT off unless VPN active; all Prowlarr indexers disabled (1337x/EZTV/PirateBay/IPTorrents)
- Jackett+FlareSolverr for Cloudflare captcha solving
- API keys: caxy15.../Prowlarr&Jackett, 7241.../Sonarr, alanthya/[REDACTED]/qB
- Media: E:\Mockbuster\Media\TV + Kids Shows/Movies

## Browser Setup
- Chromium path: `C:/Users/ericc/.agent-browser/browsers/chrome-152.0.7977.64/chrome.exe`
- Pref: hidden/background by default; visible only for logins or visuals
- Use `--headless` or `--headless=new`

## Unbroker Process
- pdd.py at `$HERMES_HOME/skills/security/unbroker/scripts/pdd.py`
- Reliable fire path: `render-email subject broker [--listing URL]` → drafts in `$HERMES_HOME/unbroker/drafts/{b}.txt` → himalaya smtp send from draft file
- ~52 brokers scanned: ~9 opt-out, 2 indirect, ~7 not found, ~27+ blocked by anti-bot

## User Profile
- Name: Eric Robert Centella (aliases: Eric Centella, Eric R Centella)
- DOB: 7/7/1984 | Phone: 352-346-4414
- Emails: ecentellahermes@gmail.com, ericcentella@live.com, minax69@hotmail.com
- Addresses: Spring Hill FL (current), Weeki Wachee + Brooksville FL (prior)

## Retirement Goal
- 5 years or less via trading profits
- Primary focus: crypto swing trades + short-term bullish signals
- Stocks lead crypto direction — use as leading indicators
- Paper trading first; proven track record before real money allocation

## Hermes Harness
- Surfaces: desktop Electron, web dashboard, Ink TUI w/ widgets
- Orchestration: delegate_task subagents, cronjob scheduler, kanban board
- Config: toolsets per session, model/provider override, context compression, checkpoints
- Voice: STT (faster-whisper/Groq/OpenAI), TTS (edge/elevenlabs/openai/minimax/mistral/gemini/piper)

## GitHub Account
- Username: ecentella-7x9k2m | Email: ecentellahermes@gmail.com
- Password: Hrm3s!Gh@ct0p#2025$Secure!
- Token: `[REDACTED]` (full repo scope)
- gh CLI: `C:/Users/ericc/.local/bin/gh.exe` — use GH_TOKEN env var
- Repo: ecentella-7x9k2m/projects

## Backtest Engine
- Workspace path: `workspace/backtest_engine.py`
- Sum of returns (not compounding) for volatile assets; handle NoneType in zero-trade strategies

## Hermes Skill Hub
- Location: `autonomous-ai-agents:hermes-agent`
- Key refs: background-systems, configuration, webhooks, providers-and-models, cli-reference, slash-commands, project-context-files, security-privacy, native-mcp, themes, desktop-plugins, tui-widgets, petdex, troubleshooting, windows-quirks
