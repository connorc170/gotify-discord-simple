I take no credit - please use the upstream fork (unless the "from gotify" message also bugs you 


Using `docker compose`:

```yaml
services:
  gotify-discord:
    image: ghcr.io/johnwiseheart/gotify-discord:latest
    container_name: gotify-discord
    environment:
      - GOTIFY_HOST=<hostname>
      - GOTIFY_TOKEN=<token>
      - DISCORD_WEBHOOK=<webhook>
    restart: unless-stopped
```

## Build it yourself

1. Clone repo
2. Run `yarn build`
3. Run `yarn start`
