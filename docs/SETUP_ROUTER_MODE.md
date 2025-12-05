# Netgear AX1800 – Router / AP Mode

This guide covers using a Linux host plus the Netgear Nighthawk AX1800 as a **Wi‑Fi access point** (router/AP role).

## 1. Prerequisites

- Linux host with at least two interfaces:
  - WAN/uplink (e.g., `eth0`).
  - Wi‑Fi interface provided by the AX1800 (e.g., `wlan0`).
- `hostapd`, `dnsmasq`, and `iptables` or `nftables` installed.

## 2. hostapd Configuration

Example file: `router/hostapd/example-ax1800-hostapd.conf`

Update the following in your private copy:

- `interface=wlan0` (or your actual Wi‑Fi interface).
- `ssid=YOUR_AP_SSID_HERE`.
- `wpa_passphrase=YOUR_STRONG_PASSPHRASE_HERE`.

## 3. dnsmasq Configuration

Example file: `router/dnsmasq/example-dnsmasq.conf`

Adjust the subnet, range, and interface to match your LAN design. Do not commit any real IP assignments that could be sensitive.

## 4. systemd-networkd

Example files:

- `router/systemd-networkd/example-wan.network`
- `router/systemd-networkd/example-lan-ap.network`

Use these as patterns for WAN DHCP and LAN static addressing.

## 5. Security Notes

- Use strong passphrases and modern cipher suites.
- Keep firmware and kernel drivers patched.

---

<p align="center">
  <sub>
    Maintained by Polymath Global / CodeSentinel, stewarded by <code>joediggidyyy</code> (Joe Waller).
  </sub>
</p>
