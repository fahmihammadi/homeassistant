# Home Assistant on K3s (Fahdin Labs)

GitOps-managed deployment of Home Assistant Core on K3s for `home.fahdin.id`.

## Architecture
- **Namespace:** `homeassistant`
- **PVC:** 10Gi on `local-path` mounted to `/config`
- **Reverse Proxy:** Traefik Ingress Controller (`ingressClassName: traefik`)
- **Public Domain:** `https://home.fahdin.id` via Cloudflare Tunnel
- **GitOps:** ArgoCD Application `homeassistant`
