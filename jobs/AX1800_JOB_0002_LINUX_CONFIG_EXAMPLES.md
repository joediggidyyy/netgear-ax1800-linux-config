# AX1800-JOB-0002 – Add Linux Configuration Templates

- **Project:** Netgear AX1800 Linux Config
- **Owner:** joediggidyyy
- **Agent:** ORACL-Prime
- **Status:** planned
- **Created:** 2025-12-04

---

## 1. Objective

Provide initial, fully redacted Linux network configuration examples for connecting to an AX1800 router, covering:

- NetworkManager
- `wpa_supplicant`
- `systemd-networkd`

---

## 2. Scope

- Add example files containing placeholders (e.g., `YOUR_SSID_HERE`, `YOUR_PASSPHRASE_HERE`).
- Document how to adapt each example for a real environment.
- Confirm the examples are syntactically valid for their respective tools.

---

## 3. Tasks

### 3.1 NetworkManager

- [ ] Create `linux/networkmanager/example-wifi-profile.nmconnection` with placeholders.
- [ ] Include comments indicating:
  - Where to put SSID.
  - Security settings (WPA2/WPA3 examples).
  - Any MTU or DNS tweaks relevant to AX1800.

### 3.2 wpa_supplicant

- [ ] Create `linux/wpa_supplicant/example-wpa_supplicant.conf`.
- [ ] Include:
  - Example `network {}` block with placeholders.
  - Notes on `proto`, `key_mgmt`, `pairwise`, `group`.

### 3.3 systemd-networkd

- [ ] Create `linux/systemd-networkd/example-wlan0.network`.
- [ ] Include:
  - DHCP vs static examples (commented).
  - Hints for integration with `wpa_supplicant` or iwd.

---

## 4. Risks / Considerations

- Examples must not contain real SSIDs, passwords, or other sensitive fields.
- Some distros may have slightly different defaults; note these when discovered.

---

## 5. Validation Checklist

- [ ] Files are valid text and load without syntax errors in their respective tools (basic sanity check).
- [ ] All examples use placeholders (`YOUR_SSID_HERE`, etc.).
- [ ] `README.md` references these examples and points users to the right directory.

---

## 6. Artifacts

- `linux/networkmanager/example-wifi-profile.nmconnection`
- `linux/wpa_supplicant/example-wpa_supplicant.conf`
- `linux/systemd-networkd/example-wlan0.network`
