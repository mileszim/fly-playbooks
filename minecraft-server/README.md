# Minecraft on Fly.io

For more configuration options, see: https://docker-minecraft-server.readthedocs.io/en/latest/variables/

## Instructions

1. Launch fly app: `fly launch --no-deploy`
2. Allocate dedicated IPs:

   ```bash
   fly ips allocate-v6
   fly ips allocate-v4 --yes
   ```

3. Launch the app: `fly deploy`
