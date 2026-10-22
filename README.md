# Star Nest — downloads

Offline DXF / SVG nesting and G-code generation for CNC plasma tables, for
CandCNC / CommandCNC and LinuxCNC / PlasmaC.

This repository holds **released installers only — there is no source code
here.** Get the newest build from the [Releases page](../../releases/latest).

## Latest release — 1.0.14

| Platform | File |
| --- | --- |
| Windows 10 / 11, x64 | `Star.Nest.Setup.1.0.14.exe` |
| Linux x64, portable | `Star-Nest-1.0.14-x86_64.AppImage` |
| Debian / Ubuntu, x64 | `starnest_1.0.14_amd64.deb` |

## Installing

**Windows** — run the installer. It is not code-signed, so SmartScreen will
show *"Windows protected your PC"*. Choose **More info**, then **Run anyway**.

**Linux, portable** — the AppImage needs no installation, just the execute
bit:

```bash
chmod +x Star-Nest-1.0.14-x86_64.AppImage
./Star-Nest-1.0.14-x86_64.AppImage
```

**Debian / Ubuntu**:

```bash
sudo apt install ./starnest_1.0.14_amd64.deb
```

## Verifying a download

Every release ships a `SHA256SUMS-<version>.txt` listing the SHA-256 of each
installer, under the exact filename GitHub serves it as:

```bash
sha256sum -c SHA256SUMS-1.0.14.txt --ignore-missing
```

On Windows:

```
certutil -hashfile "Star.Nest.Setup.1.0.14.exe" SHA256
```

A download that drops partway through produces a hash mismatch rather than an
obvious error, so if a checksum fails, re-download before assuming the file is
bad.

## About

Star Nest is commercial software from Bulltear Industries Inc. —
<https://bulltear.com>
