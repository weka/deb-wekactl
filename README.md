# deb-wekactl

APT (Debian/Ubuntu) package repository for [`wekactl`](https://github.com/weka/goweka),
the Go-based Weka CLI.

> **Generated content — do not edit by hand.**
> The `dists/` and `pool/` trees and their signed metadata are produced by the
> release pipeline in `weka/goweka` (`scripts/build_repos.sh`) and published here
> automatically. Manual edits will be overwritten on the next release.

## What lives where

- **GitHub Pages (this repo)** serves the live APT repository — the signed
  metadata (`dists/.../Release`, `InRelease`, `Packages`) plus the **current**
  `wekactl` package under `pool/`. This is what `apt` reads.
- **[Releases](../../releases)** hold the **back-catalog** of `.deb` packages for
  every published version, as downloadable assets. `apt` does not see these; they
  are for manual download when you need a specific older build.

## Installing

The canonical, supported install path is documented with the CLI itself. Use the
Weka-provided repository URL rather than pointing `apt` at this repo's Pages URL
directly, so your configured source stays stable across hosting changes.

## Source

Packaging, signing, and publishing logic lives in
**[weka/goweka](https://github.com/weka/goweka)**. File issues and changes there,
not here.
