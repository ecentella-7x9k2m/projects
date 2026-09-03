# Astralplex — Home Media Stack

## Architecture
- **Jellyfin** (8096) — media server, stream to clients
- **Sonarr v4** (8989) — TV series management, auto-download
- **Prowlarr** (9696) — indexer manager for Sonarr/Readarr/Lidarr
- **Jackett** (9117) — proxy indexers (localhost only)
- **FlareSolverr** (8191) — Cloudflare captcha solving for Jackett
- **qBittorrent** on 192.168.50.x via ProtonVPN tunnel — dynamic WebUI port, Sonarr→qB at 192.168.50.79:{port}

## Key Configs
- DHT off unless VPN active (ProtonVPN)
- All Prowlarr indexers disabled: 1337x, EZTV, PirateBay, IPTorrents
- Jackett+FlareSolverr for Cloudflare captcha solving
- API keys: caxy15.../P&J, 7241.../Sonarr

## Media Paths
- TV + Kids Shows: E:\Mockbuster\Media\TV + Kids Shows\
- Movies: E:\Mockbuster\Media\Movies\

## Agent Behavior in This Stack
- When adding indexers to Jackett/Prowlarr, check FlareSolverr is running first (8191)
- Sonarr downloads go through qBittorrent on VPN subnet — verify tunnel before seeding
- Jellyfin libraries auto-scan on media path changes
- Use `hermes config` or direct API calls to manage services
