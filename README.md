# HaloCEPortReleases

Public feed for Halo CE Port playtest builds.

- `latest.json` at the repo root is the manifest URL launcher clients should read.
- `linux/` stores versioned runtime zips named `halo-ce-port-<version>+<build>-linux-amd64.zip`.
- Source code stays private in the separate `HaloCEPortTest` repository.

Publishing is automated from the source repo:

```bash
make publish-playtest
```
