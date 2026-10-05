# opencode-serve

[![kitshn](https://kitshn.yarden-zamir.com/b/Yarden-zamir/opencode-serve.svg)](https://opencode.yarden-zamir.com)

KitSHn recipe for running `opencode serve` behind Caddy at `https://opencode.yarden-zamir.com`.
## Runtime

- Image: `ghcr.io/anomalyco/opencode:latest`
- Command: `opencode serve --hostname 0.0.0.0 --port 4096`
- Caddy route: `opencode.yarden-zamir.com -> 127.0.0.1:4096`
- Basic auth username: `opencode`
- Basic auth password: GitHub secret `KITSHN_OPENCODE_SERVER_PASSWORD`

## Notes

This recipe deploys only `main -> prod` because it binds host port `127.0.0.1:4096` and uses a fixed public hostname.
