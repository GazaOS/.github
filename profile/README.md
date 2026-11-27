![GazaOS](https://gazaos.github.io/profile/gazaos-org-logo.svg)

# GazaOS

GazaOS is a custom Android 16.2 ROM based on **Lunaris-AOSP**, **crDroid**, and **LineageOS**, built with lightweight HyperOS-style QS & UI options while keeping builds clean and portable across devices.

- **LineageOS** & **Lunaris-AOSP** for core system, Monet, and vendor base
- **crDroid** for UI options and build/OTA tooling
- **HyperOS 4** for curated wallpapers, UI sounds, and MiSans Latin font
- **CalyxOS Datura** for per-app firewall control
- **ViPER4AndroidFX** & **Sony Dolby Atmos** for audio DSP

## Features

- HyperOS Control Center QS defaults with a 1-tap `AOSP Look Lite` switch in Gaza Lab (`Singularity`)
- Compose Settings homepage styles (`GazaOS Hybrid`, `HyperOS`, `ColorOS`, `AOSP`)
- Lock Styles Studio with HyperBlur clocks and adaptive squircle icons
- Opt-in heavy add-ons (`TARGET_INCLUDE_* ?= false`) for lean Vanilla & GMS builds
- Tuned `speed-profile` dexopt and `kawase_darkmoon` blur

## Sync

```bash
repo init -u https://github.com/GazaOS/android -b 16.2 --git-lfs
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

## Links

- Website: https://gazaos.github.io/
- Official OTA & Changelogs: https://github.com/GazaOS/OTA
- Source Changelog: https://github.com/GazaOS/changelogs
- Maintainership: https://github.com/GazaOS/official
- Issue Tracker: https://github.com/GazaOS/issue_tracker
- Telegram: https://t.me/GazaOS

## Credits

Thanks to **Lunaris-AOSP**, **LineageOS**, **crDroid**, **AxionAOSP**, **EvolutionX**, **YAAP**, and the broader Android custom ROM community.

Free Palestine.
