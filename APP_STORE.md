# TestFlight checklist — Ridgewatch

1. Confirm the live web game loads (title “Ridgewatch”, Hold the pass)
2. Set `capacitor.config.json` → `server.url` to that host
3. `npm install && npx cap add ios && npx cap sync ios` (first time only)
4. Open Xcode → Team / bundle id `com.lvlltd.ridgewatch`
5. Archive → Upload → TestFlight **only if native shell changed**
6. Internal testers: Hold the pass → place a Ballista → Send wave

**Content updates** (towers, waves, art): ship web — TestFlight picks them up on next launch. No new binary required.

Privacy: no account, no tracking. Gold/lives/best score stay on device.
