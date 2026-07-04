# deb-wekactl

APT (Debian/Ubuntu) package repository for [`wekactl`](https://github.com/weka/goweka),
the Go-based Weka CLI.

> **Generated content — do not edit by hand.**
> The `dists/` and `pool/` trees and their signed metadata are produced by the
> release pipeline in `weka/goweka` (`scripts/build_repos.sh`) and published here
> automatically. Manual edits will be overwritten on the next release.

## Installing

The canonical, supported way to install `wekactl` on Debian/Ubuntu is through
**[get.weka.io](https://get.weka.io/)**, which documents how to enable the
signed APT repository and install the package:

```sh
apt install wekactl
```

Use the repository URL from get.weka.io rather than pointing `apt` at this
repo's GitHub Pages URL directly, so your configured source stays stable across
hosting changes. Debian-based distributions verify the signed repository as a
whole (rather than signing individual packages), so installing this way also
authenticates the package.

## What lives where

- **GitHub Pages (this repo)** serves the live APT repository — the signed
  metadata (`dists/.../Release`, `InRelease`, `Packages`) plus the **current**
  `wekactl` package under `pool/`. This is the tree `apt` reads.
- **[Releases](../../releases)** hold the **back-catalog** of `.deb` packages for
  every published version, as downloadable assets. `apt` does not see these; they
  are for manual download when you need a specific older build.

## Source

Packaging, signing, and publishing logic lives in
**[weka/goweka](https://github.com/weka/goweka)**. File issues and changes there,
not here.
