# `patches.json` for a custom bundle

This folder stores the complete RVX patch set in `patches.json` format.
The file is consumed by the RVMM config generator to build custom RVX
bundles.

## How to regenerate

1. Obtain the latest upstream patches from `inotia00/revanced-patches`
   (currently synced at version `v5.13.1`).
2. Convert the upstream data to `patches.json` using `patches-json-gen.jar`.
3. Use the generated `patches.json` in this folder for the config
   generator to consume.

## Update policy

`patches.json` serves solely as a snapshot for enumerating patches when generating `config.toml`; the actual compile process always pulls the latest available patches. Consequently, the list in this file may lag behind upstream releases without affecting the version used during builds.
