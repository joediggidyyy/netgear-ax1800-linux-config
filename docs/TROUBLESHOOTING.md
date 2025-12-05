# Netgear AX1800 – Troubleshooting

Quick reference for common issues when using the AX1800 with Linux in either client or router/AP mode.

## 1. Adapter Not Detected

- Check `lsusb` to confirm the device is present.
- Verify the correct kernel module is loaded.
- Review `dmesg` for firmware or power-related errors.

## 2. Cannot See SSIDs

- Confirm regulatory domain settings (`iw reg get`).
- Ensure the adapter supports the band/channel you are using.

## 3. Connects but No Internet

- Check IP assignment on the client.
- Verify default route and DNS configuration.

## 4. AP Mode Instability

- Confirm your power supply and USB port are stable.
- Test with reduced channel width or different channel.

---

<p align="center">
  <sub>
    Maintained by Polymath Global / CodeSentinel, stewarded by <code>joediggidyyy</code> (Joe Waller).
  </sub>
</p>
