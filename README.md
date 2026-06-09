# XtreamUI 24.04 - Custom Installer

Based on masoudgb installer with emre original files.

## Install

```bash
rm -rf install.py && wget -qO install.py https://raw.githubusercontent.com/red56-code/xtream-ui-custom/main/install.py && python3 install.py
```

## Installation Type

- **MAIN** - Main server with admin panel
- **LB** - Load balancer / sub server

## Notes

- Automatically disables ufw
- MariaDB buffer pool auto-configured based on available RAM
- Reboot recommended after installation
