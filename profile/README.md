<p align="center">
  <img src="https://i.postimg.cc/yYNg3mRy/Picsart-25-06-15-00-05-32-620.jpg" alt="GazaOS Logo" width="300" style="border-radius: 16px; box-shadow: 0 4px 20px rgba(0,0,0,0.3);"/>
</p>

<h1 align="center">GazaOS</h1>

<p align="center">
  <b>A refined, high-performance, and custom-tailored Android 16.2 operating system blending stability, modern UI aesthetics, and unmatched audio superiority.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Android-16.2%20(Baklava)-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android 16.2"/>
  <img src="https://img.shields.io/badge/Base-Lunaris--AOSP-blueviolet?style=for-the-badge" alt="Base Lunaris-AOSP"/>
  <img src="https://img.shields.io/badge/Vendor-LineageOS-167C80?style=for-the-badge&logo=lineageos&logoColor=white" alt="Vendor LineageOS"/>
  <img src="https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge" alt="Status Active"/>
</p>

---

## 🌟 About GazaOS

**GazaOS** is a community-driven Android ROM built on modern Android 16.2 (Baklava). Combining a stable, rock-solid core with curated cherry-picks and distinct visual enhancements, GazaOS delivers a uniquely customized experience that is fast, smooth, and bloat-free.

GazaOS merges features, performance optimizations, and ideas cherry-picked across the Android aftermarket ecosystem:

- **LineageOS**: Rock-solid stability, device compatibility, and hardware vendor base
- **Lunaris-AOSP**: Modern Android 16 core framework, system enhancements, and upstream stability
- **crDroid Android**: Cherry-picked rich customization features, lockscreen options, and UI flexibility
- **AxionAOSP & ProtonAOSP**: Boost framework, fluid animations, and frame pacing optimizations
- **AOSPA (Paranoid Android)**: Refined maintainer interfaces, hardware diagnostics, and clean aesthetics
- **Evolution X & Project Clover**: Google Pixel feature integrations, wallpapers, and GMS support
- **DerpFest & TenXOS**: Fresh UI design inspirations and accent styling
- **YAAP (Yet Another AOSP Project)**: Low-latency responsive touch and performance tuning

---

## ✨ Features & Highlights

- **Distinct GazaOS Identity**: Custom versioning (`ro.gazaos.build.version`), build types (`Community`, `Official`), and dedicated system properties.
- **Audio Superiority**: Built-in **ViPER4AndroidFX** suite (`TARGET_INCLUDE_VIPERFX := true`) and Sony / Dolby Atmos hardware integration.
- **Display & Gaming Boost**: SurfaceFlinger frame pacing boost (`SURFACE_FLINGER_BOOST := true`), Reality Engine support, and configurable high-refresh-rate profiles (up to 120Hz).
- **Pixel Features**: Optional Pixel Launcher, Monet accent theming, Pixel sound packs, and Google Mobile Services (GMS) integration.
- **Privacy & Security**: Built-in Datura firewall prebuilts, isolated app lock, and private signing key infrastructure.
- **Battery & Thermal Management**: Advanced battery graph insights, customized power-saver profiles, and background process controls.

---

## 🚀 Getting Started

### Initializing the Repository
To initialize your local build environment with the GazaOS 16.2 manifest:

```bash
mkdir -p GazaOS && cd GazaOS
repo init -u https://github.com/GazaOS/android.git -b 16.2 --git-lfs
```

For bandwidth- or disk-optimized shallow sync:
```bash
repo init -u https://github.com/GazaOS/android.git -b 16.2 --git-lfs --depth=1
```

### Syncing Sources
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

---

## 🔨 Building GazaOS

Set up the build environment and compile for your target device:

```bash
# Set up environment
source build/envsetup.sh

# Lunch target device
lunch lineage_<device_codename>-bp4a-user

# Start building
m bacon
```

### Key Build Flags
Customize your build in your device tree or `lineage_<device>.mk`:
```make
# Include Google Mobile Services (GMS)
WITH_GMS := true

# Enable ViPER4AndroidFX
TARGET_INCLUDE_VIPERFX := true

# Enable SurfaceFlinger frame pacing boost
SURFACE_FLINGER_BOOST := true

# Enable Reality Engine display enhancements
USE_REALITY_ENGINE := true

# Maintainer string
ro.gazaos.maintainer := YourName
```

---

## 📂 Key GazaOS Repositories

| Repository | Purpose | Branch |
| :--- | :--- | :--- |
| [**android**](https://github.com/GazaOS/android) | Core source tree manifest | `16.2` |
| [**android_vendor_GazaOS**](https://github.com/GazaOS/android_vendor_GazaOS) | GazaOS vendor configurations, branding, and versioning | `16.2` |
| [**packages_apps_Settings**](https://github.com/GazaOS/packages_apps_Settings) | Customized Settings application with GazaOS rebranding | `16.2` |
| [**android_packages_apps_ViPER4AndroidFX**](https://github.com/GazaOS/android_packages_apps_ViPER4AndroidFX) | ViPER4AndroidFX audio suite | `v4a` |
| [**.github**](https://github.com/GazaOS/.github) | Public organization documentation and profile | `main` |

---

## 🤝 Credits & Acknowledgements

GazaOS is made possible by the incredible work of the open-source Android community:
- [**Lunaris-AOSP**](https://github.com/Lunaris-AOSP)
- [**LineageOS**](https://github.com/LineageOS)
- [**crDroid Android**](https://github.com/crdroidandroid)
- [**AxionAOSP**](https://github.com/AxionAOSP)
- [**Paranoid Android (AOSPA)**](https://github.com/AOSPA)
- [**Evolution X**](https://github.com/Evolution-X)
- [**DerpFest**](https://github.com/DerpFest-AOSP)
- [**ProtonAOSP**](https://github.com/ProtonAOSP)
- [**AOSP**](https://android.googlesource.com)

---

<p align="center">
  <b>GazaOS Community</b> • Built with dedication for performance and freedom.
</p>
