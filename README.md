# dms-shell-git (Prebuilt Arch Package)

Prebuilt Arch Linux package for DankMaterialShell, built automatically from upstream Git and published via GitHub Releases.

No AUR.  
No pacman repo.  
No manual builds.

---

## 📦 Package

| Package | Description |
|----------|------------|
| dms-shell-git | DankMaterialShell (Core + Quickshell Shell) |

Builds include:

- x86_64
- x86_64_v3 optimized builds (preferred)
- Built from latest upstream Git
- Automatically released via GitHub Actions

---

# 🚀 Install / Update

```bash
curl -fLO https://raw.githubusercontent.com/Ravi-Kishor/dms-shell-git/main/update-dms
chmod +x update-dms
sudo mv update-dms /usr/local/bin/update-dms
update-dms
```

---

## 🧠 What the updater does

- Checks installed version via pacman
- Fetches latest GitHub release
- Prefers x86_64_v3 build
- Falls back to generic x86_64
- Downloads and installs automatically

Interactive mode:
- Update only if newer
- Force reinstall

---

## 🏗 Build Info

- Built inside Arch container
- Stripped binaries
- x86_64_v3 builds include AVX/FMA support
- Shell installed to:

```
/usr/share/quickshell/dms
```

For customization, copy files to:

- User: `~/.config/quickshell/dms`
- System: `/etc/xdg/quickshell/dms`

---

## ⚠ Requirements

Arch Linux only.

Requires:

- quickshell (recommended x86_64_v3 build)
- pacman
- curl
- jq
- sudo
