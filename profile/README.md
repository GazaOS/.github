<p align="center">
  <img src="https://i.postimg.cc/yYNg3mRy/Picsart-25-06-15-00-05-32-620.jpg" alt="GazaOS" width="220" style="border-radius: 12px;"/>
</p>

# GazaOS

GazaOS is a custom ROM based on AOSP and Lunaris-AOSP, featuring an extensive range of customizations cherry-picked from various custom ROMs, including:

- **Lunaris-AOSP for core Android 16 base and framework changes**
- **LineageOS for vendor base, HALs, and device compatibility**
- **crDroid for various UI changes and customization features**
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
- **Built-in ViPER4AndroidFX and Dolby audio integration**
- **Customizable status bar, quick settings, and lockscreen**
- **SurfaceFlinger boost and refresh rate controls**
- **Performance optimizations and clean lightweight UX**
- **Many features from various ROMs merged together**

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

## Credits

A huge thanks to the developers of all the ROMs from which GazaOS cherry-picks features, as well as the Android open-source community for making all this possible.

---

## Community
https://t.me/GazaOS
