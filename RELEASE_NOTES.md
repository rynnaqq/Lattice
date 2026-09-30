# Lattice of the Last Light v1.0.2

A display and interface update to **Lattice of the Last Light**, the open-world science-fantasy action adventure for Windows and Android.

## What changed

- **Fullscreen by default.** Both builds now open filling your display with no title bar. Press Alt+Tab or close the window to leave.
- **Sharp text at any resolution.** Interface text and icons render at your screen's native resolution instead of being scaled up from a low internal buffer, so dialogue, menus, and the HUD stay readable from 720p to 4K.
- **Quieter notices.** Status messages are now compact lines beneath the HUD, expire after 2.6 seconds, and repeat messages are filtered out. They hide automatically during dialogue, menus, loading, and the Last Light ultimate.
- **Fixed a UI timing bug.** A district transition that finished its fade after the previous HUD was cleared could leave the touch controls in an inconsistent state.

Gameplay, story, world, audio, and saves are unchanged from v1.0.0.

## Downloads

- `Lattice-v1.0.2-windows-x86_64.zip` — portable 64-bit Windows build.
- `Lattice-v1.0.2-android-arm64.apk` — landscape Android 7.0+ build for ARM64 devices, signed with the same release key as v1.0.0 so you can install it over your existing copy.
- `SHA256SUMS.txt` — checksums for both downloads.

The Windows executable is unsigned, so SmartScreen may ask for confirmation. The Android APK is distributed directly through GitHub rather than the Play Store, so Android may require permission to install it from your browser or file manager.

## Validation status

The Windows executable was launched, checked for fullscreen coverage of its monitor with no title bar, and confirmed to exit cleanly through its native close action. Automated checks against its embedded game package passed: 50 interface-readability checks at 1920x1080 and 301 journey checks covering both endings, four puzzles, fourteen locations, both optional stories, and save, continue, and death handling.

The Android APK passed release-signature verification (v2/v3), 16 KB native alignment, package metadata, and contents checks. It is signed with the same key as v1.0.0 with a higher version code, so it installs as an update. It contains ARM64 native libraries, compiled scripts, and license notices, with no debug flag or Internet permission. No physical Android device or compatible configured emulator was available, so on-device startup, performance, display cutouts, lifecycle behavior, and audio remain unverified.

Both packages were checked for excluded editable source files, project files, tests, tools, and signing material. Compiled game resources can still be inspected or reverse-engineered; these are ordinary release builds, not encrypted packages.

## Upgrading

Install the new build over v1.0.0. Your existing save is carried forward on Windows from `%APPDATA%\Godot\app_userdata\Lattice of the Last Light`. On Android, installing the new APK keeps your private save data; uninstalling first will remove it.

## Scope

This repository contains compiled downloads, screenshots, release notes, and licensing information. Source code, project files, raw art, and signing material are not included.
