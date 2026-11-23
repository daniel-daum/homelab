# homelab

My self-hosted services. Each directory is one Docker Compose stack.

| Service                | What it does           |
| ---------------------- | ---------------------- |
| [arcane](arcane)       | Docker management UI   |
| [databasus](databasus) | Database backups       |
| [gitea](gitea)         | Git forge              |
| [infisical](infisical) | Secrets manager        |
| [newt](newt)           | Pangolin tunnel client |
| [nexus](nexus)         | Package repository     |
| [postgres](postgres)   | Shared Postgres        |
| [tranquil](tranquil)   | atproto PDS            |
| [valkey](valkey)       | Redis-compatible cache |
| [zerobyte](zerobyte)   | Volume backups         |

## Usage

```sh
cd <service>
docker compose up -d
```

Secrets are not stored in this repo. They come from encrypted `.env` files (dotenvx) and Infisical.

## Access

- Public: Pangolin
- Private: Tailscale
