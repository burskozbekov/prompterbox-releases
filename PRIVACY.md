# PrompterBox Privacy Policy

_Last updated: May 10, 2026 — Studio Mode (1.1) covered._

PrompterBox ("the app", "we", "us") is a teleprompter application for macOS. We are committed to protecting your privacy. This policy explains what data the app handles and how.

## TL;DR

**We do not collect, store, transmit, or share any personal data.** Everything stays on your Mac.

## Data Collection

PrompterBox does **not** collect any personal data, usage analytics, crash reports, or telemetry of any kind. We have no servers, no accounts, and no third-party SDKs that collect data.

## Microphone Access

PrompterBox uses your Mac's microphone to enable voice-paced scrolling — the script automatically scrolls as you speak.

- Speech recognition is performed **on-device** using Apple's built-in `SFSpeechRecognizer` framework with the `requiresOnDeviceRecognition` flag enabled.
- Your voice is **never** recorded, stored, or transmitted off your device.
- Audio buffers are processed in memory in real time and immediately discarded.
- We never receive, see, or have access to any audio.

You may revoke microphone permission at any time in **System Settings → Privacy & Security → Microphone**.

## Camera Access (Studio Mode)

Starting with version 1.1, PrompterBox includes "Studio Mode" — an optional feature that records you reading the script.

- Camera access is requested only when you open Studio Mode.
- Recording is performed locally using Apple's AVFoundation framework.
- The resulting QuickTime (.mov) file is saved to your Mac (default: `~/Movies/PrompterBox/`); you can choose a different location.
- The recording is **never** uploaded, transmitted, or shared by PrompterBox. Only you can move, share, or delete it.
- A live preview is shown via the system's WebKit `getUserMedia` API while you are setting up; the preview is not recorded or persisted.

You may revoke camera permission at any time in **System Settings → Privacy & Security → Camera**.

If you do not use Studio Mode, the camera is never accessed.

## Speech Recognition

Speech recognition is provided by Apple's on-device speech framework. Apple's privacy policy applies to its operating system services. PrompterBox does not transmit anything to Apple's servers and does not enable cloud speech recognition.

## Scripts and Documents

Any teleprompter scripts you create, paste, or import are stored **locally** on your Mac (in your user document space). They are never uploaded, synced, or shared by PrompterBox.

## Network Access

PrompterBox connects to the network only to:

- Check for application updates (HTTPS request to GitHub Releases for the direct distribution build; the Mac App Store build uses Apple's standard update mechanism).

No personal data is sent in update checks. The check consists of fetching a public version manifest.

## Children

PrompterBox is not directed at children under 13. We do not knowingly collect any data from anyone, including children.

## Third Parties

We do not use any third-party analytics, advertising, tracking, or data collection SDKs.

## Changes

If this policy changes in a future version of the app, we will publish the updated policy at this URL and update the "Last updated" date.

## Contact

For privacy questions, open an issue at https://github.com/burskozbekov/prompterbox-releases/issues or contact the developer via the support URL listed on the App Store product page.
