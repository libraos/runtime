# LibraOS Runtime

Public binaries of the `libraos` CLI, the command-line entry to [LibraOS](https://libraos.com), an enterprise AI operating system that runs in your own environment.

This repository holds releases only. The source is private; each release here is mirrored from the private build.

## Install

```sh
curl -fsSL https://libraos.com/install.sh | sh
```

The installer downloads the latest release from this repository and checks it against `SHA256SUMS`. More options are on the [download page](https://libraos.com/download/).

## Download by hand

Each [release](https://github.com/libraos/runtime/releases) has:

| File | What it is |
|---|---|
| `libraos-linux-amd64`, `libraos-linux-arm64` | the CLI |
| `libraos-prompts.tar.gz`, `libraos-prompts.sha256` | the prompt pack and its checksum |
| `libraos-THIRD-PARTY-NOTICES.md` | licenses of bundled software |
| `SHA256SUMS` | checksums of every file |

The newest stable build is always at `https://github.com/libraos/runtime/releases/latest/download/<file>`. Verify a download with:

```sh
sha256sum -c SHA256SUMS --ignore-missing
```

Weekly builds are published as pre-releases.

## Related

- [libraos/engine](https://github.com/libraos/engine): LibraOS Core, which runs and coordinates coding agents on your machines.
- [libraos/next](https://github.com/libraos/next): LibraOS Next, an IDE for working with coding agents.
- [libraos/sdk](https://github.com/libraos/sdk) and [libraos/stack](https://github.com/libraos/stack): the SDK and the reference deployment.
- [Docs](https://libraos.com/docs/) · [Report a problem](https://github.com/libraos/community/issues)

This repository was called `libraos/releases` until 2026-11-24. Links to that name redirect here.
