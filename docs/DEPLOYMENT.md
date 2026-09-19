# Deployment & Operations Guide: Crypto Trading OS

## 🚀 Live Access & URLs
- **Live Public Access URL:** [/preview/prod-crypto-trading-os-69abc3/](/preview/prod-crypto-trading-os-69abc3/)
- **Internal Port:** `0`
- **Runtime Engine:** `python_preview`
- **Deployment Status:** `DEPLOYED / ACTIVE`
- **Timestamp:** `2026-09-19T16:16:16.283022+00:00`

## 🛠️ Management & Service Control
### Launch Command
```bash
python3 app.py --port 0
```

### Health Check Probe
```bash
curl -I http://127.0.0.1:0/
```

### Systemd Service Template
```ini
[Unit]
Description=Crypto Trading OS Service
After=network.target

[Service]
Type=simple
WorkingDirectory=/tmp/pytest-of-root/pytest-0/test_product_creation_and_stat0/workspaces/prod-crypto-trading-os-69abc3
ExecStart=/usr/bin/python3 /tmp/pytest-of-root/pytest-0/test_product_creation_and_stat0/workspaces/prod-crypto-trading-os-69abc3/app.py
Restart=always
RestartSec=3

[Install]
WantedBy=multi-user.target
```

## 🔒 Production Security Protocols
- HTTP-only reverse proxy via Nexus Gateway.
- Dedicated port allocation with zero port conflict.
