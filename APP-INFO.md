# Pixel Recall iOS App — Info

## App Store Connect
- **App Name**: Pixel Recall
- **Bundle ID**: `com.geekmagnetinc.pixelrecall`
- **Apple ID**: TBD — fill after App Store Connect entry exists
- **SKU**: pixel-recall-ios
- **Primary Language**: English (U.S.)
- **Platform**: iOS

## Apple Developer
- **Team ID**: L52G64VBAZ
- **Account Holder (Owner)**: Kristin Boster (kristin@kristinboster.com)
- **Developer (Chandler)**: hero88go@gmail.com — under Kristin's account
- **Company**: Geek Magnet Inc

## Codemagic
- **Project**: pixel-recall-ios (TODO: create)
- **Repo**: github.com/Hero88go/pixel-recall-ios (TODO: create)
- **Provisioning Profile name**: `pixel-recall-profile`
- **Distribution Cert name**: `pixel-recall-distribution`

## Local Setup (one-time, on this Windows box)
```
cd "c:/Users/Chandler/NEW project/pixel-recall-ios"
npm install
npx cap add ios
npx cap sync ios
```

## Asset Pipeline
- Replace `assets/icon.png` with a 1024x1024 PNG branded for Pixel Recall (currently a placeholder copied from tempo-ios)
- Then: `npx @capacitor/assets generate --ios`

## Web Source
- Source HTML: `c:/Users/Chandler/NEW project/pixel-recall.html`
- iOS-shipped copy: `www/index.html` (viewport patched for safe-area-inset)
- When you update the source, copy back into `www/index.html` and re-apply the iOS viewport meta tags.

## App Store Description (draft)
**Subtitle**: Pixel pattern memory game
**Description**:
A pixel art pattern flashes on screen. Recreate it from memory.
How far can you go before your brain gives out?

## Notes
- Pure local game — no backend.
- No accounts, no analytics yet.
