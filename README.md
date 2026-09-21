# RaceSnap AI (iOS)
Native Swift/UIKit WKWebView wrapper for https://www.racesnapai.com/ — bundle ID `ai.racesnap.app`.

## Build
Push to `main` (or Actions → iOS Build → Run workflow). Download the `RaceSnapAI-unsigned` artifact:
- `RaceSnapAI-unsigned.ipa` – unsigned device build; must be signed before installing on an iPhone (e.g. sideloading tools that sign with your free Apple ID).
- `RaceSnapAI-simulator.app.zip` – runs only in the iOS Simulator.

## Replacing branding
- App icon: `RaceSnapAI/Assets.xcassets/AppIcon.appiconset/AppIcon.png` (1024x1024 PNG, no transparency)
- Launch logo: `RaceSnapAI/Assets.xcassets/LaunchLogo.imageset/logo.png`

## Signed builds (optional)
Set repo variable `ENABLE_SIGNING=true` and add secrets: `IOS_CERT_P12_BASE64`, `IOS_CERT_PASSWORD`, `IOS_PROFILE_BASE64`, `IOS_PROFILE_NAME`, `APPLE_TEAM_ID`, `KEYCHAIN_PASSWORD`. Requires a paid Apple Developer account (development profile including your iPhone's UDID).
