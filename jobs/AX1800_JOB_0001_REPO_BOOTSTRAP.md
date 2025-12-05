# AX1800-JOB-0001 – Repository Bootstrap

- **Project:** Netgear AX1800 Linux Config (`netgear-ax1800-linux-config`, public)
- **Owner:** joediggidyyy
- **Agent:** ORACL-Prime
- **Status:** planned
- **Created:** 2025-12-04
- **Last Updated:** 2025-12-04

---

## 1. Objective

Create a public GitHub repository containing **safe, redacted** configuration patterns and documentation for using a Netgear Nighthawk AX1800 router with Linux systems.

---

## 2. Scope

**In scope:**

- Creating the public repository.
- Adding:
  - `README.md`
  - Initial directory stubs: `router/`, `linux/`, `docs/`
- Ensuring no secrets or sensitive identifiers are present.

**Out of scope (future jobs):**

- Importing real router exports (even redacted) without review.
- Vendor-specific support.

---

## 3. Tasks

- [ ] Create GitHub repo `netgear-ax1800-linux-config` (public).
- [ ] Add `README.md` based on the AX1800 config README draft.
- [ ] Create empty (or stub) directories:
  - [ ] `router/`
  - [ ] `linux/networkmanager/`
  - [ ] `linux/wpa_supplicant/`
  - [ ] `linux/systemd-networkd/`
  - [ ] `docs/`
- [ ] Add `.gitkeep` or stub `.md` files as needed so directories are tracked.
- [ ] Commit and push to `main`.
- [ ] Manually re-check repo contents for secrets (SSIDs, passwords, MACs, IPs).

---

## 4. Risks / Considerations

- Accidental inclusion of real configuration exports containing sensitive data.
- Misleading instructions if firmware/driver versions are not documented.

---

## 5. Validation Checklist

- [ ] Repo is public and reachable.
- [ ] `README.md` clearly states scope and “no secrets” policy.
- [ ] Directory structure matches the plan.
- [ ] No secrets found by manual inspection (and optionally by basic secret scanners).

---

<p align="center">
  <sub>
    Maintained by Polymath Global / CodeSentinel, stewarded by <code>joediggidyyy</code> (Joe Waller).
  </sub>
</p>
