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

Paste your Unbiased API key when the app asks. If you already use the [CLI](https://github.com/circuitandchisel/unbiased-cli-releases) and have run `unbiased login`, the app finds that key and just asks you to confirm it.

Need a key? Create one in the [dashboard](https://platform.unbiased.ai) — and set the workload's Pareto rollout to 100% so every request routes to Pareto.

The Pareto engine ships inside the app; there is nothing else to install.

## About this repository

This repo hosts **release builds and the installer only**; development happens in a private repository. Found a problem? Open an issue here, or reach us at [unbiased.ai](https://unbiased.ai).
