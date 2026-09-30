# Reclaim CLI

Release archives of the Reclaim command line. This repository holds only the
releases. The source is private.

## Install

With Homebrew:

```sh
brew tap mobile-club/reclaim
brew install reclaim
```

Without Homebrew, download the archive for your machine from the
[latest release](https://github.com/mobile-club/reclaim-cli/releases/latest)
and extract it. On an Apple silicon Mac:

```sh
mkdir -p ~/.local/opt
tar -xzf reclaim-<version>-darwin-arm64.tar.gz -C ~/.local/opt
export PATH="$HOME/.local/opt/reclaim/bin:$PATH"
reclaim version --output human
```

Each archive carries its own Node runtime. Each release publishes a
`SHA256SUMS` file to check the download.

The CLI reads nothing from Reclaim without a Reclaim credential. Ask your
Reclaim administrator for an account, then run `reclaim auth login`.
