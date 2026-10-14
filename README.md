# Luminol

<img src="assets/LuminolLogo.png" alt="Luminol" width="420">

Brightness and cursor controls for Mac.

**[Download for macOS](https://github.com/dylanwlim/luminol-updates/releases/latest)** · [All releases](https://github.com/dylanwlim/luminol-updates/releases) · [Get help](mailto:dylan@wlim.work)

Requires macOS 13 or later. Supports Apple silicon and Intel Macs.

**Luminol 1.5.2** adds a native app window with Brightness, Cursor, and About icon tabs, compact sizing, and aligned settings rows. Keep Awake and its closed-lid helper are removed pending Developer ID signing. Brightness and cursor controls retain the 1.5.1 fixes.

## Install

1. Download the **.dmg** from the latest release and open it.
2. Quit any running copy using its Luminol menu bar icon (a sun in the older Lumen release).
3. Drag the app into **Applications**, replacing the older copy if prompted.
4. Open it from Applications.
5. Choose your brightness settings or open the **Cursor** tab.

This release is Apple Development signed and is not notarized. Developer ID signing is pending. If macOS blocks the first launch, follow [Apple's instructions](https://support.apple.com/en-us/102445) for opening a downloaded app you trust using **Open Anyway**. Keep download quarantine and macOS security settings enabled. Managed Macs may restrict installation.

## Controls

| Control | Use it to |
| --- | --- |
| Brightness | Adjust normal display brightness. |
| Extra dimming | Make the picture darker than the normal minimum. |
| Extra brightness | Try an experimental brightness boost on supported XDR displays. |
| Cursor | Change the pointer's fill, border, and size. |
| Reset | Clear brightness effects and restore the earlier level where available. |

Display support varies. The nit reading is an estimate, and extra brightness may affect color or HDR video.

**Cursor changes remain after quitting.** Use **Reset cursor** to restore the defaults. Cursor controls require optional Full Disk Access, a broad macOS permission. You can use **Pointer Settings** instead; brightness controls do not require that permission.

## Keep your settings

Enable **Restore my last settings** to remember your display choices. Enable **Open at login** if you want the app to start when you sign in.

Brightness effects clear when you sleep, lock, or quit. With restoration enabled, your saved settings return when supported.

## App window

Choose **More > Open Luminol Window** from the star menu to open the app window. Use the icon tabs for **Brightness**, **Cursor**, and **About**.

Keep Awake is unavailable until Developer ID signing is available. This release includes no closed-lid helper.

## Update

Choose **Check for Updates** in About or from the app's menu bar menu. If an update is available, choose **Install & Relaunch**, or postpone it until later.

**If you use the development-signed 1.5.0 release or an earlier preview, install the latest DMG manually once.** Those copies cannot reliably start the updater. Version 1.5.1 includes the fix for later automatic updates.

Keep the app in Applications with the filename supplied by the download. If an older copy cannot update, install the latest download manually once.

## Help and removal

For a quick brightness reset, use **Control + Option + Command + 0** or choose **Reset** from the app's menu bar menu. If a display control is unavailable, use macOS Display Settings.

Before uninstalling, use **Reset cursor** if you want the default pointer, turn off **Open at login**, and turn off **Restore my last settings**. Quit the app, then delete it from Applications.

Preferences stay on your Mac. The Read Me included with the download has additional setup and recovery guidance.

[Report a problem](mailto:dylan@wlim.work) with your app version, macOS version, Mac or display model, and steps to repeat it. Remove personal information from screenshots.

Made by [Dylan](https://dylanwlim.com).
