# Netgear AX1800 – Client Mode (USB Adapter)

This guide shows how to use the Netgear Nighthawk AX1800 as a **USB Wi‑Fi adapter** on Linux. All examples use placeholders – never commit real credentials.

## 1. Prerequisites

- A Linux system with USB 3.0 port.
- AX1800 USB adapter connected.
- Appropriate kernel driver or vendor module installed.
- Basic familiarity with NetworkManager or `wpa_supplicant`.

## 2. NetworkManager Example

Example profile: `adapter/networkmanager/example-wifi-client.nmconnection`

Key fields to update in your private copy:

- `ssid=YOUR_SSID_HERE`
- `psk=YOUR_PASSPHRASE_HERE`

After copying and editing the file, place it under `/etc/NetworkManager/system-connections/` with the correct permissions, then reload NetworkManager.

## 3. wpa_supplicant Example

Example config: `adapter/wpa_supplicant/example-wifi-client.conf`

Update the `network {}` block with your real SSID and passphrase in your private copy, then point `wpa_supplicant` at the file.

## 4. Driver / Distro Notes

Use `adapter/notes/DRIVER_COMPATIBILITY.md` in the public repo to document:

- Kernel versions tested.
- Distros where the adapter works out of the box.
- Any special firmware packages required.

---

<p align="center">
  <sub>
    Maintained by Polymath Global / CodeSentinel, stewarded by <code>joediggidyyy</code> (Joe Waller).
  </sub>
</p>
