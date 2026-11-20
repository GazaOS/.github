<p align="center">
  <img src="https://i.postimg.cc/yYNg3mRy/Picsart-25-06-15-00-05-32-620.jpg" alt="GazaOS Logo" width="300" style="border-radius: 12px;"/>
</p>

<h1 align="center">GazaOS (Android 16.2)</h1>

<p align="center">
  <b>A refined, lightweight, and high-performance custom ROM based on Lunaris-AOSP and LineageOS.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Android-16.2%20(Baklava)-3DDC84?style=flat-square&logo=android&logoColor=white" alt="Android 16.2"/>
  <img src="https://img.shields.io/badge/Base-Lunaris--AOSP-blueviolet?style=flat-square" alt="Lunaris-AOSP"/>
  <img src="https://img.shields.io/badge/Manifest-16.2-orange?style=flat-square" alt="Manifest 16.2"/>
  <img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Active"/>
</p>

---

## 📖 About GazaOS

GazaOS is a community-driven Android custom ROM project focused on delivering a clean, responsive, and bloat-free user experience. Following the streamlined, modular architecture seen in projects like **aosPB-Project**, GazaOS maintains only essential core customizations directly while leveraging upstream **Lunaris-AOSP** and **LineageOS** for rock-solid stability and modern Android 16 platform support.

### ✨ Highlights
* **Android 16.2 Base**: Built on the latest Android 16 (Baklava) source tree (`refs/tags/android-16.0.0_r4` + Lineage 23.2).
* **Minimalist Architecture**: Focused repository structure avoiding unnecessary clutter and maintenance bloat.
* **Audio Superiority**: Built-in **ViPER4AndroidFX** (`TARGET_INCLUDE_VIPERFX := true`) and Sony/Dolby hardware integration.
* **Display & Performance**: SurfaceFlinger frame pacing boost, Reality Engine display support, and high-refresh-rate profile support.
* **Security & Network**: Datura firewall prebuilt support and private signing keys support.

---

## 🚀 Getting Started

### Initializing the Manifest
To initialize your local build tree with the GazaOS 16.2 manifest:

```bash
mkdir -p GazaOS && cd GazaOS
repo init -u https://github.com/GazaOS/android.git -b 16.2 --git-lfs
```

For bandwidth or disk-constrained setups (shallow sync):
```bash
repo init -u https://github.com/GazaOS/android.git -b 16.2 --git-lfs --depth=1
```

### Syncing the Source Tree
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

---

## 🔨 Building GazaOS

Set up the build environment and select your target device:

```bash
source build/envsetup.sh
lunch lineage_<device_codename>-bp4a-user
m bacon
```

*(Alternatively, standard shortcuts `breakfast <device_codename>` and `brunch <device_codename>` remain supported).*

### Recommended Build Flags
Configure your device makefile (`lineage_<device>.mk` or `gazaos_<device>.mk`):
```make
# Include Google Mobile Services (GApps)
WITH_GMS := true

# Include ViPER4AndroidFX
TARGET_INCLUDE_VIPERFX := true

# SurfaceFlinger Boost
SURFACE_FLINGER_BOOST := true
```

---

## 📂 Key Organization Repositories

| Repository | Description | Branch |
| :--- | :--- | :--- |
| [**android**](https://github.com/GazaOS/android) | Core source tree repo manifest | `16.2` |
| [**android_vendor_GazaOS**](https://github.com/GazaOS/android_vendor_GazaOS) | GazaOS vendor configurations, branding & versioning | `16.2` |
| [**android_packages_apps_ViPER4AndroidFX**](https://github.com/GazaOS/android_packages_apps_ViPER4AndroidFX) | ViPER4AndroidFX audio effects suite | `v4a` |
| [**.github**](https://github.com/GazaOS/.github) | Organization profile, documentation and workflow configurations | `main` |

---

## 🤝 Credits & Acknowledgements

* [**Lunaris-AOSP**](https://github.com/Lunaris-AOSP) - Upstream ROM platform and modern Android 16 additions
* [**LineageOS**](https://github.com/LineageOS) - The foundation of community Android development
* [**aosPB-Project**](https://github.com/aosPB-Project) - Minimalist organization and modular ROM structure inspiration
* [**AOSP**](https://android.googlesource.com) - Android Open Source Project
* [**CodeLinaro**](https://git.codelinaro.org) - Qualcomm reference implementations and display HALs
* [**crDroid Android**](https://github.com/crdroidandroid) - Legacy base and customization references
* [**Evolution X**](https://github.com/Evolution-X) & [**PixelOS-AOSP**](https://github.com/PixelOS-AOSP) - Feature inspirations
