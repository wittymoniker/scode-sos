# sOS GitHub Release ZIP Series — 2026-09-10

This release is divided into logical ZIP archives so every upload remains below 25 MB.
The archives are complementary, not byte-split fragments.

## Archives

1. `sOS_CURRENT_20260910_GITHUB_01_CORE_SOURCE.zip`
   - top-level release documentation and metadata
   - build/install scripts
   - profiles and target definitions
   - full `source/` tree, including the synchronized sCode source/runtime copy

2. `sOS_CURRENT_20260910_GITHUB_02_BOOT_RUNTIME.zip`
   - `iso-root/` boot tree
   - `dist/` initramfs images and checksums

3. `sOS_CURRENT_20260910_GITHUB_03_GROOVEBOX_BUNDLES.zip`
   - current Groovebox compatibility/reference package
   - sGroovebox stable release ZIP/TAR.GZ/checksum

4. `sOS_CURRENT_20260910_GITHUB_04_SCODE_BUNDLE.zip`
   - bundled stable sCode ZIP/TAR.GZ/checksum

## Reconstruct the complete release tree

Create an empty directory and extract all four ZIP archives into that same directory.
They all share the same top-level folder name, `sOS_CURRENT_20260910`, and their payload paths are complementary.

Linux/macOS example:

```sh
mkdir sOS-release
cd sOS-release
unzip ../sOS_CURRENT_20260910_GITHUB_01_CORE_SOURCE.zip
unzip ../sOS_CURRENT_20260910_GITHUB_02_BOOT_RUNTIME.zip
unzip ../sOS_CURRENT_20260910_GITHUB_03_GROOVEBOX_BUNDLES.zip
unzip ../sOS_CURRENT_20260910_GITHUB_04_SCODE_BUNDLE.zip
```

Then follow `sOS_CURRENT_20260910/START_HERE.md`.

The file `sOS_CURRENT_20260910_GITHUB_SERIES_SHA256SUMS.txt` verifies the GitHub-series archives themselves.
