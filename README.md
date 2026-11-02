# Luminol

<img src="assets/LuminolLogo.png" alt="Luminol" width="420">

Native display, pointer and click controls for Mac.

**[Download Luminol 1.6.2](https://github.com/dylanwlim/luminol-updates/releases/tag/v1.6.2)** · [All releases](https://github.com/dylanwlim/luminol-updates/releases) · [Historical stable 1.5.4](https://github.com/dylanwlim/luminol-updates/releases/latest)

## Install once to enable future updates

**Users of every version through 1.6.0 must manually install 1.6.1 or later once. The current download is 1.6.2 build 19. Already using 1.6.1? Choose Check for Updates.** The original update-signing key is unavailable. This version adopts a replacement pinned Ed25519 key and the separate v2 channel. After that installation, **Check for Updates** can verify and install later higher-build releases from that channel. Preferences are retained. Older apps cannot automatically trust the replacement key.

The app has an ad-hoc hardened integrity seal but **no Apple-issued signing identity or notarization**. Update signatures are separate from Apple trust: macOS may block launch or require renewed permission approval after ad-hoc replacements. Fresh-recipient acceptance and physical Intel runtime are not verified. The original latest-release channel remains on historical 1.5.4; use the current download link above.

Requires macOS 13 or later. The application contains Apple silicon and Intel binaries. No account, advertising, telemetry or subscription is required by Luminol.

### What’s new in 1.6.2

- Command-comma opens Settings, Command-W closes the front window, and standard Edit shortcuts work in text fields. About shows both version and build.
- Autoclicker pause and permission-loss feedback updates promptly even with long intervals, without sending early clicks or skipping the start delay.
- Less repeated display polling, cleaner inactive accessibility state, stricter update-download checks, and safer recovery from an interrupted release.
- Uses the same v2 update-signing key as 1.6.1. Existing v2 users can update normally; no new manual trust transition is needed.

### Included controls

- A Cursor autoclicker with a three-second start delay, a saved interval from 20 to 3,600,000 ms, and a customizable saved start/stop shortcut. F6 is the default; some keyboards require Fn–F6.
- A live menu header showing applied extra-brightness and dimming percentages, customized pointer size and colors, and the autoclicker’s active state and interval. It identifies multiple displays, wraps longer combinations and omits inactive/default settings—including an off autoclicker. Header resizing waits until slider drags end.
- Native settings with Brightness, Cursor and About tabs, compact controls, direct Settings and Updates menu actions, and clearer permission/error guidance.
- Exclusive shortcut registration, one toggle per press, and fixes for shortcut recording and recovery.

## Install

1. Download **Luminol-1.6.2.dmg** from the 1.6.2 release (or the ZIP).
2. Quit any older Luminol/Lumen copy using its menu bar menu.
3. Drag **Luminol.app** into **Applications**, then open it there. Preserve the supplied app filename.
4. Choose settings from the star menu. Existing preferences are retained.

If macOS offers **Open Anyway** for an app you trust, follow [Apple’s documented steps](https://support.apple.com/en-us/102445). Keep Gatekeeper and download quarantine enabled. Some Macs, including managed devices, may refuse this unsigned release. The included SHA-256 checksums verify integrity, not Apple trust.

Stable 1.5.4 is Apple Development signed but is also not notarized. A Developer ID-signed/notarized release is still pending.

## Controls and permissions

| Control | Behavior | Permission |
| --- | --- | --- |
| Brightness | Changes the normal display brightness. Normal keyboard brightness keys remain available. | No click-control or Full Disk Access permission required. |
| Extra dimming | Darkens the picture below the normal minimum. | None of the above. |
| Extra brightness | Experimental XDR boost on supported built-in displays; macOS and hardware limit output. | None of the above. |
| Pointer appearance | Changes fill, border and size. Changes persist after quitting; Reset cursor restores defaults. | Optional **Full Disk Access**, a broad permission. Use Pointer Settings instead if you prefer. |
| Autoclicker | Left-clicks at the system pointer after a delay. Interval and shortcut are remembered; running state is never restored. | **Accessibility**, called **Device Control and Data Access** on newer macOS. |

Approve the installed app, then quit and reopen when macOS requests it. Ad-hoc replacement builds may require permissions to be approved again. Pointer appearance and click control use separate permissions.

Clicking pauses while Luminol is active, its menus are open, or a mouse button is held. Sleep, lock, permission loss and quit stop it; wake never restarts it. Use the selected shortcut or the switch to stop. Reserved shortcuts may be unavailable. Timing is best effort when macOS is busy.

Display support varies. Nit values are estimates, not light-meter measurements. Extra brightness can affect color/HDR video and power use. Keep Awake and its privileged helper are not included.

## Settings and recovery

Choose **Settings…** directly from the star menu. In Brightness, **Restore my last settings** remembers display choices; **Open at login** starts the app after sign-in and may need Login Items approval. These are separate options.

Brightness effects clear on sleep, lock and quit. Saved effects return only when restoration is enabled. After an interrupted session, automatic restoration is paused until you explicitly choose settings again.

Use **Reset** or **Control + Option + Command + 0** (top-row zero) to clear brightness effects and restore the earlier level where available. Pointer reset is separate. macOS Display Settings and Pointer Settings remain available as fallbacks.

## Updates

1. Manually download and install **1.6.1 or later once**, quitting the old copy first. Approve macOS permissions for the exact installed app when required.
2. For subsequent releases, choose **Check for Updates** from the star menu or About, then **Install & Relaunch** when offered. Display preferences, shortcut and interval are retained; clicking never starts on launch.

Version 1.6.1 uses independently signed manifests in [channels/v2](channels/v2). Both the manifest and exact ZIP must verify against its pinned public key. Only newer builds can install. The public key is `zyovtSprgraUVqtJKL2dEfm2djuTUGHPvzZOUvW/CWI=`; no private key is included. An up-to-date result means no newer build is currently published on that channel. GitHub CDN propagation may briefly delay discovery.

The original `/releases/latest` feeds remain at 1.5.4 for old-key installations. They do not deliver 1.6.1. Historical releases and their assets remain unchanged. The old signing-key loss is why this one manual trust transition is required, including for 1.6.0 users.

**macOS approval remains separate:** an unsigned replacement may need launch approval and renewed click-control/Full Disk Access. Future Apple-signed releases may also require approval when identity changes. Keep Gatekeeper and quarantine enabled; managed Macs may prohibit unsigned software. This channel does not promise unattended acceptance on every Mac.

## Privacy, help and removal

Preferences stay on your Mac. Update checks contact GitHub only when requested; no display preferences or identities are sent. The app includes no privileged daemon. The bundled Read Me contains additional setup and recovery details.

To remove Luminol, reset the cursor if desired, turn off Open at login and Restore my last settings, quit, and delete the app from Applications.

[Report an issue](mailto:dylan@wlim.work) with the app/macOS versions, Mac or display model, and reproduction steps. Remove personal information from screenshots.

Made by [Dylan](https://dylanwlim.com). MIT licensed. This public repository hosts downloads and documentation; application source remains private.
