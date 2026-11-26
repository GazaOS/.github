<div align="center">

# GazaOS

**HyperOS-Hybrid Lite AOSP 16.2 · Free Palestine Solidarity**

[![Website](https://img.shields.io/badge/Website-gazaos.github.io-0B6B4D?style=for-the-badge)](https://gazaos.github.io/)
[![Manifest](https://img.shields.io/badge/Manifest-16.2-10B981?style=for-the-badge)](https://github.com/GazaOS/android)
[![Telegram](https://img.shields.io/badge/Community-t.me%2FGazaOS-0088cc?style=for-the-badge)](https://t.me/GazaOS)

</div>

GazaOS is a hybrid custom ROM built on AOSP 16.2, combining core upstream bases from **Lunaris-AOSP**, **crDroid**, and **LineageOS** with **GazaOS** system styling, **HyperOS-Hybrid** visuals, **Gaza Lab** customization, and a Free Palestine humanitarian solidarity mission.

## Core ROM Repositories

- [`android`](https://github.com/GazaOS/android) (`16.2`): Main ROM manifest (`snippets/gazaos.xml`) and lite build guide
- [`frameworks_base`](https://github.com/GazaOS/frameworks_base) (`16.2`): SystemUI Modular QS (rounded-square tiles, MIUI corner-spread springs), framed screenshot overlay & rounded icons, lock screen & GazaOS crest integration
- [`packages_apps_Settings`](https://github.com/GazaOS/packages_apps_Settings) (`16.2`): Compose bento Homepage (`Hybrid` / `HyperOS` / `ColorOS` / `AOSP` presets), device-badged About tile, Bento About Phone card, and GazaOS Dev Info
- [`packages_apps_Singularity`](https://github.com/GazaOS/packages_apps_Singularity) (`16.2`): **Gaza Lab** customization hub (QS Mist defaults, status bar icon bar & GazaOS crest logo, lock screen clock/styles, Monet, gestures)
- [`vendor_lineage`](https://github.com/GazaOS/vendor_lineage) (`16.2`): GazaOS branding/props (`ro.gazaos.ui=HyperOS-Hybrid`), HyperOS squircle icon mask & rounded signal/Wi-Fi bar overlays, lightweight HyperOS 4 media (`GazaOSWallpapers`, audio, `MiSansLatinVF`), opt-in extra flags
- [`bootable_recovery`](https://github.com/GazaOS/bootable_recovery) (`16.2`): GazaOS Recovery & Fastbootd branded artwork and version headers
- [`android_packages_apps_ViPER4AndroidFX`](https://github.com/GazaOS/android_packages_apps_ViPER4AndroidFX) (`16.2`): Built-in ViPER4AndroidFX audio processing
- [`hardware_dolby`](https://github.com/GazaOS/hardware_dolby) (`sony-1.0`): Built-in Sony Dolby Atmos HAL & audio integration
- [`prebuilts_calyx_datura`](https://github.com/GazaOS/prebuilts_calyx_datura) (`15-qpr2`): Prebuilt Calyx Datura per-app firewall
- [`vendor_lineage-priv_keys`](https://github.com/GazaOS/vendor_lineage-priv_keys) (`16.2`): Signing keys template & certificate overrides for GazaOS builds

> **Device Trees**: GazaOS focuses on clean ROM source repositories. Pair with your own device, vendor, and kernel trees (for example, Mayu trees) via `.repo/local_manifests/`.

## Highlights

- **HyperOS-Hybrid on AOSP Logic**: Preserves native Android 16.2 shade/notification flow while delivering HyperOS-inspired rounded-square QS tiles, MIUI spring animations, squircle adaptive icon masks, framed screenshot shelf cards, and pill signal/Wi-Fi icon bars.
- **Lite & Fast by Default**: Heavy optional packages (`GameSpace`, `LMOFreeform`, `BatteryStatsViewer`, `AxThemeStore`, `OmniStyle`, `MatLog`) are opt-in (`?= false`), `TARGET_LOW_END_BLUR=true`, and builds default to `speed-profile` dexopt.
- **HyperOS 4 Media**: Lightweight curated `GazaOSWallpapers` (~5 MB), HyperOS 4 lock/unlock/notification/ringtone audio, and `MiSansLatinVF`.
- **GazaOS Identity**: Custom GazaOS geometric crest across Status Bar, About Phone, Settings, Bootanimation, and Recovery/Fastbootd.

## Stand With Palestine

GazaOS stands in solidarity with the people of Palestine. Verified humanitarian relief organizations:
- **[Palestinian Red Crescent Society (PRCS)](https://www.palestinercs.org/)**
- **[Medical Aid for Palestinians (MAP)](https://www.map.org.uk/)**
- **[UNRWA](https://www.unrwa.org/)**

## Sync & Build

```bash
repo init -u https://github.com/GazaOS/android -b 16.2 --git-lfs
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
# Add your device/vendor/kernel trees (e.g. Mayu trees) into .repo/local_manifests/
. build/envsetup.sh
lunch lineage_<device_codename>-bp4a-user
m bacon
```

## Team

- **Lead Developer**: **Farhan Muh Tasim** ([@Gtajisan](https://github.com/Gtajisan) / [@frnAlt](https://github.com/frnAlt))
- **Website**: [gazaos.github.io](https://gazaos.github.io/) · **Telegram**: [t.me/GazaOS](https://t.me/GazaOS)
