# Scoop bucket for Sluice

[Sluice](https://github.com/sanamhub/sluice) sends a file straight from one computer to another.
Nothing is stored in between.

```powershell
scoop bucket add sanamhub https://github.com/sanamhub/scoop-bucket
scoop install sluice
```

The manifest installs the release binary for Windows on x86_64 or arm64. Upgrade with
`scoop update sluice` and remove with `scoop uninstall sluice`.

`sluice.json` is generated from the release's checksums by `cargo xtask package` in the Sluice
repository. Do not edit it by hand: change the template there and generate it again.
[`docs/install.md`](https://github.com/sanamhub/sluice/blob/main/docs/install.md) lists every way to
install Sluice and how to verify a download.
