# XtreamUI 24.04 - Custom Installer

Based on masoudgb installer with emre original files.

## What is different from masoudgb

From masoudgb:
- PHP 7.3 binaries and extensions (php, php-fpm)
- start_services.sh
- nginx balance.conf

Everything else is original from emre:
- nginx + nginx_rtmp (1.27.0 + OpenSSL 3.3.x)
- ffmpeg + ffprobe
- Admin panel files (release_22f)
- database.sql
- php-fpm pool configs

## Install

```bash
rm -rf install.py && wget -qO install.py https://raw.githubusercontent.com/red56-code/xtream-ui-custom/main/install.py && python3 install.py
```

## Installation Type

- **MAIN** - Main server with admin panel
- **LB** - Load balancer / sub server

## Notes

- Automatically disables ufw
- MariaDB buffer pool auto-configured based on available RAM (50%, min 1G, max 12G)
- Reboot recommended after installation
