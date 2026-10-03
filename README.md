# mycel-gh

Release downloads for `mycel-gh`, the Mycel command-line tool for GitHub Actions jobs.

`mycel-gh` runs inside CI and deploy workflows. It is not meant to be run by hand. This
repository holds release archives only. It contains no source code.

## Downloads

Each [release](https://github.com/mycelpf/mycel_cli_gh/releases) has four archives and a
checksum file:

- `mycel-gh_<version>_darwin_amd64.tar.gz`
- `mycel-gh_<version>_darwin_arm64.tar.gz`
- `mycel-gh_<version>_linux_amd64.tar.gz`
- `mycel-gh_<version>_linux_arm64.tar.gz`
- `SHA256SUMS`

Verify a download before use:

```bash
shasum -a 256 -c SHA256SUMS --ignore-missing
```

## Pinning

Workflows that use `mycel-gh` pin the exact archive URL and its SHA-256 digest. Do not rely on a
moving "latest" download.
