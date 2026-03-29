# imagineering.cc

Landing page for [imagineering.cc](https://imagineering.cc) — a single group chat bridged across five platforms.

## Platforms

- Discord
- Telegram
- WhatsApp
- Signal
- Matrix (Element)

All platforms are connected via [matrix-chat-superbridge](https://github.com/imagineering-cc/matrix-chat-superbridge). Send a message on any app and everyone sees it everywhere.

## Deploy

Merging to `main` auto-deploys to production via GitHub Actions.

For manual deploys:
```bash
# From the imagineering-infra repo
./scripts/deploy-to.sh 149.118.69.221 site
```

Served by Caddy from `/srv/site` on the OCI instance (Sydney).
