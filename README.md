# Ridgewatch — iOS / TestFlight shell

Capacitor wrapper that loads the live **Ridgewatch** tower-defense game (same pattern as Tesla Trek).

When the web build updates, TestFlight testers get it on next app open — no App Store resubmit for content.

## Play now
The game is a browser tower defense: place Ballista / Mortar / Frost Spire / Arc Coil on the mountain pass, spend gold from kills, upgrade damage and fire rate, survive 12 blight waves.

## Requirements
- macOS + Xcode 16+
- Apple Developer team (LVL LTD / your team)

## Bootstrap (once)
```bash
npm install
npx cap add ios
npx cap sync ios
npx cap open ios
```

In Xcode:
1. Set Team + bundle id `com.lvlltd.ridgewatch`
2. Signing & Capabilities → Automatic
3. Product → Archive → Distribute → TestFlight

## Config
Live URL is in `capacitor.config.json` → `server.url`.
Set it to the published Ridgewatch URL (Grok `.grok.me` host or a `lvlltd.com` domain) before the first archive.

Allowed hosts include `*.grok.me`, Vercel, and Google Fonts.
