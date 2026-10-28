# theorem releases

Prebuilt `theorem` CLI binaries. The source repository is private; this
repository only carries what installers download. Each release holds one
archive per target, a `sha256.sum` covering them, and `install.sh`.

## Install

```sh
curl -fsSL https://github.com/Travis-Gilbert/theorem-releases/releases/latest/download/install.sh | sh
```

The installer picks the archive for your platform, verifies it against
`sha256.sum`, and installs `theorem` to `~/.theorem/bin`. It never compiles
from source. `THEOREM_RELEASE_TAG` installs a specific release, and
`THEOREM_INSTALL_PREFIX` changes where it goes.

Targets: `aarch64-apple-darwin`, `x86_64-apple-darwin`,
`x86_64-unknown-linux-gnu`, `aarch64-unknown-linux-gnu`,
`x86_64-pc-windows-msvc`.

Releases are published automatically by the source repository's release
workflow. Please don't open pull requests here.
