# GazaOS

GazaOS is a hybrid custom ROM built on AOSP, combining core repositories from **Lunaris-AOSP**, **crDroid**, and **LineageOS** with **GazaOS** system logic, **HyperOS / ColorOS / GazaOS Hybrid** UI craft, **Gaza Lab** customization, and a Free Palestine humanitarian solidarity motive:

- **Website & Download Portal**: [gazaos.github.io](https://gazaos.github.io/)
- **Lunaris-AOSP & LineageOS** for core Android 16.2 base, framework, HALs, and device compatibility
- **crDroid** for UI changes, OTA JSON schema, versioning flow, and customization features
- **GazaOS core repositories (`android`, `vendor_lineage`, `frameworks_base`, `packages_apps_Settings`, `packages_apps_Singularity`, `bootable_recovery`)** for HyperOS/ColorOS/Hybrid Settings UI, Gaza Lab, unified properties, and Free Palestine solidarity
- **AxionAOSP and ProtonAOSP** for frame pacing and smoothness
- **EvolutionX and Project Clover** for Pixel features and GMS
- **ViPER4AndroidFX & Sony Dolby Atmos** for system audio processing
- **Calyx Datura** for per-app network firewall control
- **AOSPA (Paranoid Android)** for hardware diagnostics and maintainer info
- **YAAP (Yet Another AOSP Project)** for touch response and performance tuning
- **DerpFest and TenXOS** for UI ideas and styling

## Features

GazaOS brings a balanced mix of modern UI craft, performance, audio fidelity, and customization while keeping stability and lean image size in mind:

- **Android 16.2 (Baklava) base**
- **Adaptive Settings Homepage Engine**: Compose-based bento layout with live **GazaOS Hybrid**, **HyperOS**, **ColorOS**, and **AOSP** presets, squircle icon shapes, contained chevrons, and drag-and-drop tile customization
- **Modular Quick Settings (Mist QS)**: Modular header, ColorOS-style tile backgrounds, cached dynamic blur, and waveform media controls
- **Gaza Lab (`Singularity`)**: Status bar logos (including full-color Palestine flag vector), lockscreen clocks, input-monitor 3-finger swipe gestures, and Monet theming
- **Dynamic About Phone & GazaOS Dev Info**: Live hardware summary card and dedicated developer/solidarity info menu
- **Built-in ViPER4AndroidFX, Sony Dolby Atmos & Datura Firewall**
- **Optimized `speed-profile` dexopt, content-detection refresh rate controls, and clean lightweight UX**

## 🇵🇸 Stand With Palestine

GazaOS is dedicated to freedom, human dignity, and solidarity with the people of Palestine.

If you would like to support humanitarian relief efforts on the ground, consider donating to verified international organizations:
- **[Palestinian Red Crescent Society (PRCS)](https://www.palestinercs.org/)**: Emergency medical and ambulance services in Gaza and the West Bank.
- **[Medical Aid for Palestinians (MAP)](https://www.map.org.uk/)**: Critical health and medical support for Palestinians.
- **[UNRWA](https://www.unrwa.org/)**: United Nations Relief and Works Agency providing emergency aid, food, and shelter.

## Build

Initialize local repository:
```bash
repo init -u https://github.com/GazaOS/android -b 16.2 --git-lfs
```

Sync:
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

Build:
```bash
. build/envsetup.sh
lunch lineage_<device_codename>-bp4a-user
m bacon
```

## Team & Maintainers

- **Lead Developer**: **Farhan Muh Tasim** ([@Gtajisan](https://github.com/Gtajisan) / [@frnAlt](https://github.com/frnAlt))
- **Device Maintainer (`stone`)**: **Masud Parvez** ([@Parvez52](https://github.com/Parvez52))

## Credits

A huge thanks to the developers of all the ROMs from which GazaOS cherry-picks features, as well as the Android open-source community for making all this possible.

---

## Community
- **Website**: https://gazaos.github.io/
- **Telegram**: https://t.me/GazaOS
