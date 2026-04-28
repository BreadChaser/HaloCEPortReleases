# HaloCEPortReleases

Public feed for Halo CE Port playtest builds.

- `latest.json` at the repo root is the manifest URL launcher clients should read.
- `linux/` stores versioned runtime zips named `halo-ce-port-<version>+<build>-linux-amd64.zip`.
- `windows/` is reserved for future Windows packages.
- `launcher/` is reserved for standalone launcher builds.
- Each package entry includes system, architecture, filename, executable name, version, build, and build name while keeping `packages.<platform>.url` simple for launchers.
- `latest.json` sets `resource_dir` to `resources`; launchers should create that folder beside the versioned runtime folders and keep player-owned Halo files there across updates.
- Source code stays private in the separate `HaloCEPortTest` repository.

Publishing is automated from the source repo:

```bash
make publish-playtest
```
