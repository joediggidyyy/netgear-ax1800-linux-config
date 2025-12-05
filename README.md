# Netgear AX1800 Linux Config

Public reference repository for a Netgear Nighthawk AX1800 USB adapter / router running with Linux.

> This repo contains **redacted examples and documentation only**. Do not store real SSIDs, passwords, MAC addresses, or public IPs here.

## Layout

- `adapter/` – client-mode configurations when using the AX1800 as a USB Wi‑Fi adapter.
  - `networkmanager/` – NetworkManager profiles (`*.nmconnection`).
  - `wpa_supplicant/` – `wpa_supplicant.conf` examples.
  - `notes/` – driver / distro compatibility notes.
- `router/` – Linux host acting as router/AP using the AX1800.
  - `hostapd/` – example `hostapd.conf` for AP mode.
  - `dnsmasq/` – example `dnsmasq.conf` for DHCP/DNS on the Wi‑Fi LAN.
  - `systemd-networkd/` – `*.network` examples for WAN/LAN.
- `docs/` – higher-level guides and troubleshooting.
- `assets/images/` – optional tiny branding assets (e.g., Polymath logo) referenced only from footers.

## Getting Started

1. Copy this entire directory into your `netgear-ax1800-linux-config` repo root.
2. Review each example and replace placeholders like `YOUR_SSID_HERE` and `YOUR_PASSPHRASE_HERE` **in your own private copies only**.
3. Never commit real credentials or identifying information back to the public repo.

## Attribution

<p align="center">
  <sub>
    Maintained by Polymath Global / CodeSentinel, stewarded by <code>joediggidyyy</code> (Joe Waller).
  </sub>
</p>
