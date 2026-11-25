# XrayN

XrayN is a Linux-focused desktop client based on the v2rayN/Avalonia codebase, with Xray, sing-box and Aether runtime integration.

## Manjaro / Arch Linux

Two x86_64 packages are provided:

- **Pacman package:** install with `sudo pacman -U XrayN-linux-x86_64.pkg.tar.zst`
- **AppImage:** make executable with `chmod +x XrayN-linux-x86_64.AppImage`, then run it.

The pacman package installs the application under `/opt/xrayn`, registers the `xrayn` launcher and adds an application-menu entry.

## Local build

Run on Manjaro or Arch Linux with the .NET 10 SDK and `base-devel` installed:

```bash
./package-arch.sh --buildfrom 3 --netcore --with-core both
```

The script packages the current checkout and does not perform a full system upgrade.

## Licensing

This project retains the upstream GPL license and third-party notices. See `LICENSE` and the files under `licenses/`.
