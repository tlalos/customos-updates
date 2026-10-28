# Custom OS updates

Update channel for the Custom OS taskbar.

This repository holds only:

| File | What it is |
|---|---|
| `update.json` | Latest taskbar version: version code/name, APK address, size, SHA-256, notes, minimum image |
| `update.json.sig` | Ed25519 signature of `update.json` |
| `apk/` | Taskbar APK files |
| `LICENSE`, `NOTICE` | Apache License 2.0 and notices for Taskbar |

The taskbar checks the signature with its built-in public key before it reads `update.json`,
and checks the APK's SHA-256 before it installs. An unsigned or changed file is ignored.

## Licence

The taskbar is a modified build of [Taskbar](https://github.com/farmerbb/Taskbar) by Braden Farmer,
licensed under the Apache License 2.0. See [LICENSE](LICENSE) and [NOTICE](NOTICE).
