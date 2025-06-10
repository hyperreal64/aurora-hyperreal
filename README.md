# aurora-hyperreal

This is my custom build of UBlue OS Aurora. It isn't anything remarkable.

## Features

- [Aurora features](https://docs.getaurora.dev#features)
- [VSCodium](https://vscodium.com/)
- borgmatic
- btrfs-assistant
- Prometheus node-exporter
- Firefox (non-flatpak)

In contrast to the default Aurora settings, the following systemd units are disabled by default in this build:

- bluetooth.service
- bolt.service
- cups.service
- wpa_supplicant.service
- zfs-mount.service
- zfs-share.service
- zfs-zed.service

## Installation

```shell
sudo bootc switch --enforce-container-sigpolicy ghcr.io/hyperreal64/aurora-hyperreal:latest
sudo systemctl reboot
```
