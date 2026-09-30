# Ableton Silent Mode

![Latest release](https://img.shields.io/github/v/release/SimonHolden/ableton-silentmode?include_prereleases)

A small Windows tray app that keeps Ableton Live launching silently after unattended restarts, with no crash recovery dialogs and nobody needing to click anything.

## Why this exists

If Ableton Live gets killed unexpectedly (a power cut, a forced reboot, a remote restart), it leaves a marker behind that makes it show a crash recovery dialog the next time it opens. That's fine if someone's sitting at the machine to click through it. It's a real problem if the machine is meant to come back up and start playing on its own with nobody there, which is exactly the situation for unattended installs: venues, galleries, art installations, anything running Ableton as part of a show with no human standing by.

Ableton Silent Mode runs quietly in the system tray, clears that crash recovery state before Ableton ever opens, and also silences Windows Error Reporting so a crash doesn't throw up its own popup either. The result is Ableton Live starting clean, every time, with nobody watching.

## What it does

- Clears Ableton's crash recovery flag before launch, silently.
- Suppresses Windows Error Reporting dialogs for Ableton Live specifically, not system wide.
- Archives, never deletes, any crash state it clears, so nothing is lost if you ever want to look back at what happened.
- Runs as a small tray icon with two presets: Normal (plain ring icon) for stock Ableton behaviour when you're at the machine yourself, and Silent (crossed-out speech bubble icon) for a fully locked down unattended rig.
- Works with any edition of Ableton Live (Intro, Standard, Suite), since it detects the install rather than assuming one.
- Installs as a proper Windows app: Start Menu entry, registers itself to launch at logon with the right privileges, and uninstalls cleanly without touching your saved settings.

## Installing

Grab the latest installer from the [Releases page](https://github.com/SimonHolden/ableton-silentmode/releases), run it, done. Re-running the installer later to update won't touch your existing settings or activity log.

Still in beta, so expect the odd rough edge. Use it at your own risk: it runs well on my own rigs, but there's no warranty, so test it on your own setup before trusting it on a show.

## Questions or bugs?

Open an [issue on GitHub](https://github.com/SimonHolden/ableton-silentmode/issues) and I'll take a look.

## Support

Ableton Silent Mode is free to use. If it's saved you from a dead unattended rig, or just made your installs a little less nerve wracking, why not consider supporting it by buying me a cup of joe.

[![Buy Me A Coffee](https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png)](https://buymeacoffee.com/sintech)

---

Built by Simon, Sinclair Technology. Queenstown / Wanaka, New Zealand.
