# Lattice of the Last Light v1.0.0

The first public release of **Lattice of the Last Light** is a complete open-world science-fantasy action adventure for Windows and Android.

## Highlights

- One continuous city with fourteen named locations, connected roads, shortcuts, neighborhoods, woodland, gardens, wildlife, and optional discoveries.
- Directional melee, dash, pulse, shield, Lattice Spear, Orbit Break, and a fully animated three-second Last Light ultimate.
- Five enemy types, four mechanisms, two optional stories, and two conclusions shaped by the journey.
- Painted environments and characters, an illustrated travel-journal interface, district ambience, an original arranged score, layered fantasy combat effects, and spoken casting callouts.
- Persistent saves, map waypoints, keyboard and touch controls, reduced motion, separate volume controls, and Low / Medium / High graphics presets.

## Downloads

- `Lattice-v1.0.0-windows-x86_64.zip` — portable 64-bit Windows build.
- `Lattice-v1.0.0-android-arm64.apk` — landscape Android 7.0+ build for ARM64 devices, signed with the project's release key.
- `SHA256SUMS.txt` — checksums for both downloads.

The Windows executable is unsigned, so SmartScreen may ask for confirmation. The Android APK is distributed directly through GitHub rather than the Play Store, so Android may require permission to install it from your browser or file manager.

## Current validation status

The Windows executable was launched and its native window-close action exited cleanly. Automated checks against its embedded game package passed for the complete journey, both endings, saves, world geometry, terrain, population, combat, skills, casting audio, graphics settings, and rendered effects. Nine world views were captured.

The Android APK passed release-signature verification (v2/v3), alignment, package metadata, and contents checks. It contains ARM64 native libraries, compiled scripts, and license notices, with no debug flag or Internet permission. No physical Android device or compatible configured emulator was available, so on-device startup, performance, display cutouts, lifecycle behavior, and audio remain unverified.

Both packages were checked for excluded editable source files, project files, tests, tools, and signing material. Compiled game resources can still be inspected or reverse-engineered; these are ordinary release builds, not encrypted packages.

## Scope

This repository contains compiled downloads, screenshots, release notes, and licensing information. Source code, project files, raw art, and signing material are not included.

Saves from development builds are not guaranteed to migrate to this public release. On Android, uninstalling the app can remove its private save data.
