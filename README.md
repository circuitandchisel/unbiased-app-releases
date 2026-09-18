# Unbiased desktop

The [Unbiased Pareto](https://unbiased.ai) coding agent as a Mac app — projects, worktrees, diff review, a built-in terminal and browser, and approval controls, all on Pareto.

## Install

```bash
curl -fsSL https://raw.githubusercontent.com/circuitandchisel/unbiased-app-releases/main/install.sh | bash
```

Downloads the latest release, verifies its SHA-256, installs `Unbiased.app` to `/Applications`, and clears the download quarantine flag so it opens on the first try.

Prefer doing it by hand? Download the `.dmg` from [Releases](https://github.com/circuitandchisel/unbiased-app-releases/releases/latest), drag **Unbiased** to Applications, then **right-click → Open** the first time. That one-time step is needed because the app is ad-hoc signed rather than notarized; the installer script does it for you.

## Requirements

- **Apple Silicon Mac** (M1 or newer) — there is no Intel build
- **macOS 12** (Monterey) or newer

## First launch

Choose **Sign in with browser** to select an existing Unbiased workload. You
can also paste an Unbiased API key; if the
[CLI](https://github.com/circuitandchisel/unbiased-cli-releases) has already
saved one, the app finds it and asks you to confirm it.

Need an account or workload? Start at the
[Unbiased platform](https://platform.unbiased.ai).

The Pareto engine ships inside the app; there is nothing else to install.

## Source

This repository hosts release builds and the installer. Development happens
in the public source repositories:

- [unbiased-app](https://github.com/circuitandchisel/unbiased-app)
- [unbiased-app-engine](https://github.com/circuitandchisel/unbiased-app-engine)
- [unbiased-ax](https://github.com/circuitandchisel/unbiased-ax)

Found a problem? Open an issue here, or visit [unbiased.ai](https://unbiased.ai).

## License

Repository source is licensed under Apache-2.0. See [LICENSE](LICENSE) and
[NOTICE](NOTICE). The Unbiased name and logo are covered separately by
[TRADEMARKS.md](TRADEMARKS.md). Release assets include their own third-party
notices inside the application bundle.
