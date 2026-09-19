# Contributing

This repository contains the public installer and release metadata for
Unbiased desktop. Product changes belong in the source repositories:

- [unbiased-app](https://github.com/circuitandchisel/unbiased-app)
- [unbiased-app-engine](https://github.com/circuitandchisel/unbiased-app-engine)
- [unbiased-ax](https://github.com/circuitandchisel/unbiased-ax)

Pull requests here should be limited to the installer, release documentation,
or repository maintenance. Validate changes with:

```bash
bash -n install.sh
```

Do not add release binaries directly to Git. Official assets are produced by
the release workflow and published through GitHub Releases.

By submitting a contribution, you agree that it may be distributed under
the repository's Apache-2.0 license. Report vulnerabilities through
[SECURITY.md](SECURITY.md), not a public issue.
