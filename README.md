# Luminol

<img src="assets/LuminolLogo.png" alt="Luminol" width="420">

Native display, pointer and click controls for Mac.

**[Download 1.6.0 unsigned public preview](https://github.com/dylanwlim/luminol-updates/releases/tag/v1.6.0)** · [Stable 1.5.4 download](https://github.com/dylanwlim/luminol-updates/releases/latest) · [All releases](https://github.com/dylanwlim/luminol-updates/releases)

## 1.6.0 public preview

Build 17 is a **manual-download prerelease without an Apple-issued signing certificate or notarization**. It has an ad-hoc integrity seal, which is not Apple developer trust. macOS may block or refuse launch. Fresh-recipient acceptance and Intel runtime have not been verified. The existing signed automatic-update channel remains on 1.5.4.

Requires macOS 13 or later. The application contains Apple silicon and Intel binaries. No account, advertising, telemetry or subscription is required by Luminol.

### What’s new

- A Cursor autoclicker with a three-second start delay, a saved interval from 20 to 3,600,000 ms, and a customizable saved start/stop shortcut. F6 is the default; some keyboards require Fn–F6.
- A live menu header showing applied extra-brightness and dimming percentages, customized pointer size and colors, and the autoclicker’s active state and interval. It identifies multiple displays, wraps longer combinations and omits inactive/default settings—including an off autoclicker. Header resizing waits until slider drags end.
- Native settings with Brightness, Cursor and About tabs, compact controls, direct Settings and Updates menu actions, and clearer permission/error guidance.
- Exclusive shortcut registration, one toggle per press, and fixes for shortcut recording and recovery.

## Install

1. Download **Luminol-1.6.0.dmg** from the preview release (or the ZIP).
2. Quit any older Luminol/Lumen copy using its menu bar menu.
3. Drag **Luminol.app** into **Applications**, then open it there. Preserve the supplied app filename.
4. Choose settings from the star menu. Existing preferences are retained.

If macOS offers **Open Anyway** for an app you trust, follow [Apple’s documented steps](https://support.apple.com/en-us/102445). Keep Gatekeeper and download quarantine enabled. Some Macs, including managed devices, may refuse this unsigned preview. The included SHA-256 checksums verify integrity, not Apple trust.

Stable 1.5.4 is Apple Development signed but is also not notarized. A Developer ID-signed/notarized release is still pending.

## Controls and permissions

| Control | Behavior | Permission |
| --- | --- | --- |
| Brightness | Changes the normal display brightness. Normal keyboard brightness keys remain available. | No click-control or Full Disk Access permission required. |
| Extra dimming | Darkens the picture below the normal minimum. | None of the above. |
| Extra brightness | Experimental XDR boost on supported built-in displays; macOS and hardware limit output. | None of the above. |
| Pointer appearance | Changes fill, border and size. Changes persist after quitting; Reset cursor restores defaults. | Optional **Full Disk Access**, a broad permission. Use Pointer Settings instead if you prefer. |
| Autoclicker (1.6 preview) | Left-clicks at the system pointer after a delay. Interval and shortcut are remembered; running state is never restored. | **Accessibility**, called **Device Control and Data Access** on newer macOS. |

Approve the installed app, then quit and reopen when macOS requests it. Ad-hoc replacement builds may require permissions to be approved again. Pointer appearance and click control use separate permissions.

Clicking pauses while Luminol is active, its menus are open, or a mouse button is held. Sleep, lock, permission loss and quit stop it; wake never restarts it. Use the selected shortcut or the switch to stop. Reserved shortcuts may be unavailable. Timing is best effort when macOS is busy.

Display support varies. Nit values are estimates, not light-meter measurements. Extra brightness can affect color/HDR video and power use. Keep Awake and its privileged helper are not included.

## Settings and recovery

Choose **Settings…** directly from the star menu. In Brightness, **Restore my last settings** remembers display choices; **Open at login** starts the app after sign-in and may need Login Items approval. These are separate options.

Brightness effects clear on sleep, lock and quit. Saved effects return only when restoration is enabled. After an interrupted session, automatic restoration is paused until you explicitly choose settings again.

Use **Reset** or **Control + Option + Command + 0** (top-row zero) to clear brightness effects and restore the earlier level where available. Pointer reset is separate. macOS Display Settings and Pointer Settings remain available as fallbacks.

## Updates

This unsigned preview is **manual installation only**. It is not marked latest stable and has no automatic-update manifests. **Check for Updates** continues to use the existing signed stable channel. A future signed release will use a new version/build; a manual installation may be needed when changing signing identities.

Users of development-signed 1.5.0 or earlier previews need a manual stable DMG installation once to obtain the corrected updater. Published historical releases are never replaced.

## Privacy, help and removal

Preferences stay on your Mac. Update checks contact GitHub only when requested; no display preferences or identities are sent. The app includes no privileged daemon. The bundled Read Me contains additional setup and recovery details.

To remove Luminol, reset the cursor if desired, turn off Open at login and Restore my last settings, quit, and delete the app from Applications.

[Report an issue](mailto:dylan@wlim.work) with the app/macOS versions, Mac or display model, and reproduction steps. Remove personal information from screenshots.

Made by [Dylan](https://dylanwlim.com). MIT licensed. This public repository hosts downloads and documentation; application source remains private.
