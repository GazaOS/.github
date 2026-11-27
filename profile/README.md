<p align="center">
  <a href="https://gazaos.github.io/">
    <img src="https://gazaos.github.io/profile/gazaos-org-logo.svg" alt="GazaOS Organization Logo" height="72" />
  </a>
</p>

<p align="center">
  <a href="https://gazaos.github.io/">Website</a> &bull;
  <a href="https://github.com/GazaOS/android">Manifest (16.2)</a> &bull;
  <a href="https://github.com/GazaOS/OTA">Official OTA</a> &bull;
  <a href="https://github.com/GazaOS/changelogs">Changelogs</a> &bull;
  <a href="https://github.com/GazaOS/official">Maintainership</a> &bull;
  <a href="https://github.com/GazaOS/issue_tracker">Issue Tracker</a> &bull;
  <a href="https://t.me/GazaOS">Telegram</a>
</p>

---

# GazaOS — HyperOS-Hybrid Lite Android 16.2

**GazaOS** is an open-source Android 16.2 (`BP4A`) custom ROM combining upstream stability from **Lunaris-AOSP**, **crDroid**, and **LineageOS** with a modular **HyperOS Control Center QS**, a one-tap **AOSP Look Lite** toggle in **Gaza Lab**, lightweight HyperOS 4 media/fonts, and a **Free Palestine** humanitarian solidarity mission.

## Core Repositories & Organization Management

| Repository | Purpose | Link |
| :--- | :--- | :--- |
| **Platform Manifest** | Sync all GazaOS 16.2 source trees (`repo init -b 16.2`) | [GazaOS/android](https://github.com/GazaOS/android) |
| **Official OTA** | Device OTA manifests (`builds/`, `builds/vanilla/`) & device changelogs | [GazaOS/OTA](https://github.com/GazaOS/OTA) |
| **Source Changelogs** | Platform-wide dated feature & security patch changelogs | [GazaOS/changelogs](https://github.com/GazaOS/changelogs) |
| **Official Maintainership** | Standards, code of conduct, device roster & application form | [GazaOS/official](https://github.com/GazaOS/official) |
| **Issue Tracker** | User bug reports, crash logs & feature triage | [GazaOS/issue_tracker](https://github.com/GazaOS/issue_tracker) |
| **Official Website** | Device downloads, interactive UI studio & team | [gazaos.github.io](https://gazaos.github.io/) |

## Highlights

- **HyperOS Control Center & AOSP Look Lite:** Full HyperOS Control Center QS defaults (split shade, horizontal swipe, rounded-square sliders & tiles, blurred vertical GazaOS volume panel) with a one-tap **AOSP Look Lite** switch inside **Gaza Lab** (`packages_apps_Singularity`).
- **Lightweight UI & Media:** Curated HyperOS 4 wallpapers, ringtones/UI audio, MiSans Latin font, and adaptive squircle masks while heavy add-ons remain opt-in (`TARGET_INCLUDE_* ?= false`).
- **Compose Settings & Launcher3:** Live homepage layout presets (`GazaOS Hybrid`, `HyperOS`, `ColorOS`, `AOSP`), dynamic About Phone hardware cards, Lock Styles Studio, and custom Updater/SetupWizard.
- **Privacy & Audio DSP:** Built-in Calyx Datura firewall, Sony Dolby Atmos, and ViPER4Android FX.

## Quick Sync

```bash
repo init -u https://github.com/GazaOS/android -b 16.2 --git-lfs
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

## Credits

Huge gratitude to **Lunaris-AOSP**, **LineageOS**, **crDroid**, **AxionAOSP**, **DerpFest**, **EvolutionX**, **YAAP**, **CalyxOS (Datura)**, and all open-source device maintainers.

---

<p align="center">❤️ Free Palestine 🇵🇸 &bull; Released under the Apache 2.0 License</p>
