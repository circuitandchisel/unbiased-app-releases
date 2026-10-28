# Unbiased desktop

The [Unbiased Pareto](https://unbiased.ai) coding agent as a Mac app — projects, worktrees, diff review, a built-in terminal and browser, and approval controls, all on Pareto.

## Install

```bash
curl -fsSL https://raw.githubusercontent.com/circuitandchisel/unbiased-app-releases/main/install.sh | bash
```

Downloads the latest release (large: about 470 MB at v1.13.25; the script prints the size first), verifies its SHA-256, installs `Unbiased.app` to `/Applications`, and clears the download quarantine flag. If it ends with "download failed", run the same command again; it resumes.

Prefer doing it by hand? Download the `.dmg` from [Releases](https://github.com/circuitandchisel/unbiased-app-releases/releases/latest), drag **Unbiased** to Applications and open it. The first time, macOS says it cannot verify the app and offers only Move to Trash or Done: click **Done**, open **System Settings > Privacy & Security**, scroll to Security, click **Open Anyway**, then open Unbiased again (on macOS 14 and earlier, right-click > Open does the same). That one-time step is needed because the app is ad-hoc signed rather than notarized. The installer script clears the download flag; if the warning still appears, the same fix applies.

## Requirements

- **Apple Silicon Mac** (M1 or newer) — there is no Intel build
- **macOS 12** (Monterey) or newer

## First launch

Click **Sign in with your browser** and finish on the page that opens; there
is nothing to copy or paste. Invited by your company? Accept the invitation
email first, then sign in with that email. Developers can instead choose
"Have an API key? Paste it instead"; if the
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
