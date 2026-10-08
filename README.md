# Luminol

Luminol is the new name of Lumen. The latest available download is still **Lumen 1.4.0 (build 7)**, published September 25, 2026. The Luminol app branding and Keep Awake features are being prepared for a future release and are not included in that download. Existing published binaries, checksums and signatures are unchanged.

Simple brightness and cursor controls for your Mac: normal brightness, extra dimming, experimental XDR brightness boost on supported displays, and optional system cursor color, border, and size controls.

[Download the current release (Lumen 1.4.0)](https://github.com/dylanwlim/lumen-updates/releases/latest)

## Install the current release

1. Download the `.dmg` from the latest release and open it.
2. Quit any older Lumen copy from its sun menu, then drag Lumen into Applications, replacing the old copy.
3. Open Lumen from Applications. Current builds are ad-hoc signed, not Apple Developer ID signed or notarized. If macOS blocks the app, use **System Settings > Privacy & Security > Open Anyway** after your first launch attempt, only for a copy you trust. Do not disable system security protections.

Requires macOS 13 or later. Includes Apple silicon and Intel support. Display features vary by Mac and connected screen; the nit count is an estimate, not a measured or guaranteed output.

## Cursor controls

The Cursor tab controls cursor fill, border, and size. Changes affect the macOS pointer and remain after Lumen quits. Use **Reset cursor** to restore the default colors and size before uninstalling when needed. Apps that draw their own cursor may not follow these settings.

Lumen's optional cursor controls require Full Disk Access. That permission grants broad local file access; brightness controls do not require it. You can leave the permission off and use **Pointer Settings** instead. If cursor controls are unavailable on your Mac, brightness controls remain usable. The Read Me included in the DMG describes tested hardware and macOS coverage.

## Name change and compatible updates

The project is now called Luminol. This repository intentionally keeps its `lumen-updates` address because installed apps trust that exact update channel. Keep the installed app at `/Applications/Lumen.app` or `~/Applications/Lumen.app`; do not manually rename it. A future Luminol release will display the new name while preserving the app’s update identity and existing preferences.

New disk images will use `Luminol-<version>.dmg`. The update ZIP remains `Lumen-<version>.zip`, containing `Lumen.app`, for compatibility with existing signed clients. The old filename is expected and does not mean you received the wrong app. Until that release is published, the installation and feature instructions here describe Lumen 1.4.0.

## Updates

Install the **latest published release manually once**, then use **Check for Updates** beside the version or in the sun menu. Built-in updates are supported from 1.3.1 onward; 1.3.1 is the compatibility threshold, not the version to prefer over a newer release.

Checks happen when requested, not continuously. No GitHub account or sign-in is needed. Keep the app in Applications with permission to replace it; do not edit files inside the app.

## Privacy and support

Preferences stay on your Mac. Lumen has no telemetry. An update check contacts GitHub, which receives ordinary connection information; display preferences are not sent.

The DMG's included Read Me contains the full control, restoration, recovery, and removal instructions. Describe the app version, macOS version, hardware, and reproducible behavior when reporting a problem; do not upload private logs, signing material, or personal files.

Made by [Dylan](https://dylanwlim.com).
