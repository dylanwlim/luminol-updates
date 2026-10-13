# Luminol

<img src="assets/LuminolLogo.png" alt="Luminol" width="420">

Brightness, cursor and Keep Awake controls for Mac.

**[Download for macOS](https://github.com/dylanwlim/luminol-updates/releases/latest)** · [All releases](https://github.com/dylanwlim/luminol-updates/releases) · [Get help](mailto:dylan@wlim.work)

Requires macOS 13 or later. Supports Apple silicon and Intel Macs.

**Luminol 1.5.1** repairs the menu brightness and extra-dimming controls, includes the new Luminol artwork, adds Keep Awake with closed-lid support, and corrects the signed updater.

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

## Keep Awake

Open the Luminol star menu to choose a duration, end time, indefinite session, or a session that ends when a selected app quits. **More > Open Luminol Window** opens the optional window. Right-click the star to start your saved duration or end the current session. Sessions end when you quit and do not resume on relaunch.

Closed-lid support is included. Follow setup in Awake settings and approve the helper in **System Settings > General > Login Items** when requested. Use it only when Awake settings reports ready. Development signing may restrict helper approval on other Macs. Physical lid-close operation on a fresh recipient Mac remains experimental and unverified; the built-in display turns off when closed, and external-display behavior depends on your setup.

Avoid running multiple sleep-control apps together. Battery protection ends sessions below 15% by default; high temperatures may warn or end a session. Automatic locking on lid closure may request Accessibility access and can be turned off.

## Update

Choose **Check for Updates** beside the version or from the app's menu bar menu. If an update is available, choose **Install & Relaunch**, or postpone it until later.

**If you use the development-signed 1.5.0 release or an earlier preview, install the 1.5.1 DMG manually once.** Those copies cannot reliably start the updater. Version 1.5.1 includes the fix for later automatic updates.

Keep the app in Applications with the filename supplied by the download. If an older copy cannot update, install the latest download manually once.

## Help and removal

For a quick brightness reset, use **Control + Option + Command + 0** or choose **Reset** from the app's menu bar menu. If a display control is unavailable, use macOS Display Settings.

Before uninstalling, use **Reset cursor** if you want the default pointer, turn off **Open at login**, and turn off **Restore my last settings**. End any awake session and remove closed-lid support in Awake settings. Quit the app, then delete it from Applications.

Preferences stay on your Mac. The Read Me included with the download has additional setup and recovery guidance.

[Report a problem](mailto:dylan@wlim.work) with your app version, macOS version, Mac or display model, and steps to repeat it. Remove personal information from screenshots.

Made by [Dylan](https://dylanwlim.com).
