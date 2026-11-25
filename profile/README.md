# GazaOS

GazaOS is a hybrid custom ROM built on AOSP, combining core repositories from **Lunaris-AOSP**, **crDroid**, and **LineageOS** with **GazaOS** system logic, Gaza Lab customization, and a Free Palestine humanitarian solidarity motive:

- **Lunaris-AOSP & LineageOS for core Android 16.2 base, framework, HALs, and device compatibility**
- **crDroid for UI changes, OTA JSON schema, versioning flow, and customization features**
- **GazaOS core repositories (`android`, `vendor_lineage`, `frameworks_base`, `packages_apps_Settings`, `packages_apps_Singularity`, `bootable_recovery`) for Gaza Lab, unified properties, and Free Palestine solidarity**
- **AxionAOSP and ProtonAOSP for frame pacing and smoothness**
- **EvolutionX and Project Clover for Pixel features and GMS**
- **ViPER4AndroidFX for system audio processing**
- **AOSPA (Paranoid Android) for hardware diagnostics and maintainer info**
- **YAAP (Yet Another AOSP Project) for touch response and performance tuning**
- **DerpFest and TenXOS for UI ideas and styling**
- **And many more**

## Features

GazaOS brings a balanced mix of performance, audio fidelity, and customization while keeping stability in mind. Some of its notable features include:

- **Android 16.2 (Baklava) base**
- **Pixel features and Monet theming**
- **Built-in ViPER4AndroidFX and sound enhancements**
- **Customizable status bar, quick settings, and lockscreen**
- **SurfaceFlinger boost and refresh rate controls**
- **Performance optimizations and clean lightweight UX**
- **Many features from various ROMs merged together**

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
https://t.me/GazaOS
