# homelab-k8s

Kubernetes manifests for my homelab, running on a single-node k3s cluster (HP Z440).

| App | Namespace | NodePort | Storage |
|---|---|---|---|
| MeTube | metube | 30081 | hostPath (`/mnt/media/music-staging`) |
| Uptime Kuma | uptime-kuma | 30001 | PVC (local-path) |

Ingress is handled by Caddy on the host (`*.home.lan`), with DNS via Pi-hole.
