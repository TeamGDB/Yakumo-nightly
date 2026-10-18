# Yakumo Nightly

> **Experimental development builds. Use at your own risk.** Nightly builds can contain unfinished changes, crashes, rendering bugs, performance regressions and save-data problems. **Back up your saves and settings before installing or testing a nightly.**
>
> For regular play, use the [latest stable Yakumo release](https://github.com/TeamGDB/Yakumo/releases/latest).

This repository is the download channel for nightly builds of [Yakumo](https://github.com/TeamGDB/Yakumo), the native port of *Monster Hunter Portable 3rd HD Ver.* (`NPJB-40001`). A nightly is a snapshot of development, intended for testing changes and reporting regressions before a stable release.

The source code, build workflows, development discussions and bug tracker live in [TeamGDB/Yakumo](https://github.com/TeamGDB/Yakumo). This repository hosts distribution information and ready-to-run packages.

## Downloads

- [Latest nightly](https://github.com/TeamGDB/Yakumo-nightly/releases/latest) — the newest successfully published experimental build.
- [All nightly builds](https://github.com/TeamGDB/Yakumo-nightly/releases) — previous snapshots from this channel.
- [Stable releases](https://github.com/TeamGDB/Yakumo/releases/latest) — the recommended choice for normal play.
- [Installation, controls and game-data requirements](https://github.com/TeamGDB/Yakumo/blob/main/profiles/mhp3rd/README.md).

Nightly runs are scheduled daily at **00:00 UTC**, publishing when `main` has changed since the latest complete nightly. A manual run can force a rebuild. GitHub may queue a scheduled run after that time. Packages cover Windows x86-64, Linux / Steam Deck x86-64, macOS Apple Silicon and Android ARM64.

This channel uses normal GitHub Releases marked **Latest** for convenient downloads. They remain **experimental nightlies**, without stable-release sign-off. A newer nightly is not automatically a better or more stable build. A successful build or passing automated tests does not establish that every device and gameplay scenario was tested. Publication requires all four platform packages to pass content checks and the Android APK to pass production-signature verification; failed build or verification checks block publication.

Before downloading, read that build's release notes. Check its source commit, included platforms, test results, known problems and checksums. Choose the package for your operating system and CPU architecture, and verify it against the attached `SHA256SUMS`.

## Protect your saves and settings

1. Export or back up your saves, settings and any mods or texture packs you want to keep. Store the backup outside the installation or data folder you are changing; confirm that it contains the expected files.
2. Keep a known-good stable installer and an untouched copy of your backup. Prefer a separate test installation and a copy of your data when the platform and package support it.
3. Do not assume a nightly uses separate player data. If it uses the same data folder or Android application ID as stable Yakumo, the installations share that data. A different executable or installation directory alone does not guarantee isolation.
4. On Android, export your saves before uninstalling an app or clearing its storage. Both operations can remove its private player data. Do not treat replacing an APK as a save backup.
5. If a nightly fails, return to a known-good build and use your preserved backup. Stop testing on your only copy of important saves.

Android nightlies use the normal Yakumo application ID and release signing key. They update the ordinary installation and use its existing player data.

See the upstream [save and backup guide](https://github.com/TeamGDB/Yakumo/blob/main/profiles/mhp3rd/README.md#where-saves-live-and-how-to-back-them-up), [macOS guide](https://github.com/TeamGDB/Yakumo/blob/main/docs/MACOS.md) and [Linux / Steam Deck guide](https://github.com/TeamGDB/Yakumo/blob/main/docs/LINUX.md).

## Game files are not included

You must provide the compatible game files from your own legally obtained copy of *Monster Hunter Portable 3rd HD Ver.* These downloads do not include disc images, original game executables, archives, textures, models, audio, saves or other original game assets.

Do not distribute pirated game copies or builds bundled with a game image through this repository or the project's other spaces. Follow the upstream [game-content policy](https://github.com/TeamGDB/Yakumo/blob/main/CODE_OF_CONDUCT.md#piracy-and-game-content).

## Report a bug

Report ordinary bugs and compatibility problems in the [main Yakumo issue tracker](https://github.com/TeamGDB/Yakumo/issues/new/choose). Include:

- The exact nightly release and source commit.
- Your operating system, device, CPU and GPU; relevant driver versions and settings.
- Reproduction steps, expected behavior and actual behavior.
- Whether the same problem occurs in the latest stable release, and the last working build if known.
- Relevant logs or screenshots, with personal information removed.

Do not attach game files, saves, keys, credentials or private build inputs. Follow the upstream [contributor guide](https://github.com/TeamGDB/Yakumo/blob/main/CONTRIBUTING.md) and [code of conduct](https://github.com/TeamGDB/Yakumo/blob/main/CODE_OF_CONDUCT.md). Issues are kept in the main repository so reports are not split between channels.

## Report a security vulnerability

Report suspected vulnerabilities privately using [Yakumo's vulnerability reporting form](https://github.com/TeamGDB/Yakumo/security/advisories/new), following the upstream [security policy](https://github.com/TeamGDB/Yakumo/blob/main/SECURITY.md). Do not publish exploit details in release comments or ordinary issues.

## Licenses and source offers

Yakumo's source license is in the [main repository](https://github.com/TeamGDB/Yakumo/blob/main/LICENSE). Bundled dependencies retain their own licenses; see the notices inside each package and the upstream [third-party notices](https://github.com/TeamGDB/Yakumo/blob/main/profiles/mhp3rd/packaging/THIRD_PARTY_NOTICES.md).

Each nightly release must include applicable license notices and the corresponding source archives required for its bundled dependencies, including FFmpeg when it is bundled. Game ownership and game-content requirements remain separate from the port's software license.
