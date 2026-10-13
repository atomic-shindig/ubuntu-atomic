<div align="center">
  </a>
  <br>
  <h1 align="center"><center>Ubuntu Sysupdate Remix</center></h1>
  <h3 align="center"><center>(Unofficial) Sysupdatified Ubuntu</center></h3>
  <br>
  <br>
</div>

## Building, Testing, and Installation

You'll need the following runtime dependencies:
* podman
* just
* zstd
* systemd

Generate keys and then build with `just`

```bash
just genkey
just do-release
```
Create install media with [Fedora Media Writer](https://flathub.org/en/apps/org.fedoraproject.MediaWriter) or [Impression](flathub.org/en/apps/io.gitlab.adhami3310.Impression), or boot with GNOME Boxes (>=51).

### Installation (sysupdate)

Once in the liveiso, inside the terminal or a tty, run:

```bash
sudo repart-install
```
You will be prompted with installation options.


## Operations

### Upgrades

`updatectl update`

Append the exact version ID at the end to upgrade to a specific version, or downgrade.

## Minimum specs
- UEFI with secure boot disabled
- 8 GB of USB flash drive
- GNOME Boxes >=51 (for VM only)
- 55 GB of destination disk
- 4 GB of system memory (RAM)
