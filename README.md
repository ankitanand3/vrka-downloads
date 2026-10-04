# Vrka Downloads

[Download the Mac development build](https://github.com/ankitanand3/vrka-downloads/releases/tag/v0.1.0-dev.1).

# Vrka 0.1.0 — Mac development build

These downloads contain the core Vrka desktop application. They are development
candidates, not a signed, notarized or supported consumer release. macOS may
block opening them. Do not disable security protections to run this build.

## Choose your Mac

- Apple Silicon (M-series): `Vrka-0.1.0-macos-arm64.dmg`
- Intel: `Vrka-0.1.0-macos-x64.dmg`

The intended dependency floor is macOS 13. Native packaged checks ran on macOS
15; a local Apple Silicon copy/runtime check ran on macOS 14.5. Clean consumer
installation across the intended OS/CPU range remains pending.

Each DMG has a matching `.sha256` checksum and `.json` build-provenance file.
The assets come from clean source `f8314da9eeea658ea22e1fc88a28e0acd9c61926`,
native run 37155560714. They are published unchanged and must not be replaced
under this tag. Later builds get a new versioned release.

| Mac | DMG bytes | SHA-256 |
| --- | ---: | --- |
| Apple Silicon | 63,082,301 | `9e7eab482b8b59405028e7a4a85543b0eaeec19bc4171643eccbb481633c850d` |
| Intel | 67,129,351 | `d1bd300565208dd8dda2b702f49612973edd2e0c62df1166c22cecf1813db592` |

## Install and first use

Open the DMG, drag `Vrka.app` to Applications, eject the DMG and open Vrka from
Applications. If macOS blocks it, stop; trusted Developer ID signing and Apple
notarization are still pending. No Python, Git or source checkout is required
for the installed core app.

Set Claude or OpenAI and your own funded provider API key in Vrka's settings.
Grant Screen Recording for screen-based questions. Voice/input permissions are
needed only for features that use them. Kokoro dependencies are excluded from
these core packages. Qwen requires a separately configured server and tunnel.

## What has been verified

Native build/package checks and offline first-run setup, typed-answer and
shutdown flows pass. Checksums and provenance were independently checked after
download. Apple Silicon CI payload signature integrity passes; its ad-hoc
signature does not provide Developer ID trust or notarization.

Real downloaded first use, native permissions and credential persistence,
upgrade/rollback/uninstall preservation and consumer-device qualification remain
pending. Download availability does not establish those results.

This public repository distributes development binaries and release notes.
The application's source repository remains private.
