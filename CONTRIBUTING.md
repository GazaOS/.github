# Contributing to GazaOS

Thank you for your interest in contributing to **GazaOS**! 🇵🇸

We welcome community contributions, device maintainers, bug fixes, and feature enhancements. To keep code quality high across the platform, please review the following guidelines.

---

## 1. Commit Message Guidelines

We follow standard Android open-source commit formatting:

```
module: Short imperative description in present tense

Detailed explanation of why this change is necessary and what it accomplishes.
Reference any relevant issues or pull requests.

Change-Id: I...
Signed-off-by: Your Name <your.email@domain.com>
```

### Module Prefixes
Use concise module prefixes matching the directory or subsystem:
- `manifest:` for repository entries and snippet changes
- `vendor:` for vendor configurations, roomservice, and overlay updates
- `SystemUI:` for statusbar, lockscreen, quick settings, and notifications
- `Settings:` for Settings app, Gaza Lab entries, and hardware info
- `recovery:` for bootable recovery changes
- `sepolicy:` for SELinux policy rules

### Commit Hygiene
- Keep commits **atomic**: do not combine unrelated fixes into a single commit.
- Sign your commits with a verified email matching your GitHub profile.
- Do not check in merge commits or dirty binary files.

---

## 2. Device Bringup & Maintenance

If you wish to maintain a device under the GazaOS organization:
1. Ensure your device trees, vendor trees, and kernel sources are public and clean.
2. Submit a **Device Maintainer Application** via the GitHub issue templates.
3. Test all core functionalities before submitting:
   - Boot, display refresh rate, touch response
   - Cellular calls, VoLTE, mobile data, SMS
   - Wi-Fi, Bluetooth, GPS
   - Camera, flashlight, audio, microphone
   - Hardware keys, biometrics (fingerprint / face unlock)
   - Encryption, recovery, and OTA packages

---

## 3. Upstream Patches

To maintain stability without maintaining 80+ heavy forks, code modifications for un-forked upstream repositories (`Lunaris-AOSP` / `LineageOS`) are applied via the patch manager:
- Place patch files in `vendor/lineage/patches/<relative_path_with_underscores>/`
- Verify patches apply cleanly with `vendor/lineage/apply-patches.sh`

---

## 4. Palestine Solidarity

GazaOS proudly supports humanitarian relief and human dignity for the people of Palestine. Contributions, documentation, and maintainer bios must adhere to respectful community standards.
