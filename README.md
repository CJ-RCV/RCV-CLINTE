<div align="center">

<img width="100%" alt="RCV Client — Official Purple Banner" src="https://raw.githubusercontent.com/CJ-RCV/RCV-CLINTE/main/assets/rcv-banner.png" />

### A new look. A smoother experience. Your Minecraft, your style.

**RCV Client** is a custom **Fabric client** for **Minecraft Java 1.21.11**, featuring a rich purple interface, practical UI improvements, a selection of gameplay modules, and direct access to the RCV community.

<p>
  <img alt="Version 1.0.0" src="https://img.shields.io/badge/VERSION-1.0.0-8B5CF6?style=for-the-badge&amp;labelColor=181026"/>
  <img alt="Minecraft 1.21.11" src="https://img.shields.io/badge/MINECRAFT-1.21.11-A78BFA?style=for-the-badge&amp;labelColor=181026"/>
  <img alt="Fabric" src="https://img.shields.io/badge/LOADER-FABRIC-8B5CF6?style=for-the-badge&amp;labelColor=181026"/>
  <img alt="Beta" src="https://img.shields.io/badge/STATUS-BETA-B45309?style=for-the-badge&amp;labelColor=181026"/>
</p>

<a href="https://github.com/CJ-RCV/RCV-CLINTE/releases/download/v1.0.0/RCV-Client-1.0.0.jar">
  <img alt="Download RCV Client 1.0.0" src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-RCV%20CLIENT%201.0.0-7C3AED?style=for-the-badge&amp;logo=github&amp;logoColor=white"/>
</a>
<a href="https://rcv-mc.bond">
  <img alt="Official RCV website" src="https://img.shields.io/badge/%F0%9F%8C%90%20OFFICIAL%20WEBSITE-RCV--MC.BOND-4C1D95?style=for-the-badge"/>
</a>

<br/><br/>

[**Download**](#-download) · [**Features**](#-features) · [**Install**](#-installation) · [**Compatibility**](#-compatibility) · [**FAQ**](#-frequently-asked-questions) · [**Support**](#-support--links)

</div>

---

## ✨ Discover RCV Client

<table>
<tr>
<td width="50%" valign="top">

### 💜 Purple by design
A coordinated violet theme across the **main menu, ClickGUI, HUD accents, window title, and music interface**. Appearance stays customizable through the client's controls.

</td>
<td width="50%" valign="top">

### ⚡ Practical optimizations
Targeted changes reduce redundant UI drawing, unnecessary allocations, color-picker draw calls, and inactive-window resource usage.

</td>
</tr>
<tr>
<td valign="top">

### 🎮 Gameplay tools
Explore the original client's **Combat, Movement, Render, World, and Utility** modules. Configure features for your own gameplay or permitted servers.

</td>
<td valign="top">

### 🌐 Connected to RCV
A dedicated **RCV-MC.BOND** button opens the official site directly from the client's main menu.

</td>
</tr>
</table>

> [!NOTE]
> Performance changes are source-level optimizations, **not a guarantee of a particular FPS increase**. Results depend on your device, resolution, settings, and enabled modules.

## ⬇️ Download

<div align="center">

### RCV Client **v1.0.0** · Purple Edition

| Package | Minecraft | Channel | Download |
|:--|:--:|:--:|:--|
| **RCV-Client-1.0.0.jar** | **1.21.11** | **Beta** | **[Get the JAR](https://github.com/CJ-RCV/RCV-CLINTE/releases/download/v1.0.0/RCV-Client-1.0.0.jar)** |

**[View release information →](https://github.com/CJ-RCV/RCV-CLINTE/releases/tag/v1.0.0)**

</div>

<details>
<summary><b>🔐 File verification (SHA-256)</b></summary>

After downloading, you can verify the release file with this checksum:

```text
f3a20f9753dc503d50ed189076353a8dec796052731cb52cec0bcfc0ed934216
```

Windows PowerShell:

```powershell
Get-FileHash .\RCV-Client-1.0.0.jar -Algorithm SHA256
```

Linux / macOS:

```bash
sha256sum RCV-Client-1.0.0.jar
```

The output should match the checksum above.

</details>

## 🛠️ Installation

1. Install **Minecraft Java Edition 1.21.11**.
2. Install **[Fabric Loader](https://fabricmc.net/use/installer/)** for 1.21.11 (Loader **0.19.3** or a compatible newer version).
3. Install the matching **[Fabric API](https://modrinth.com/mod/fabric-api)** for Minecraft 1.21.11.
4. Download **[RCV-Client-1.0.0.jar](https://github.com/CJ-RCV/RCV-CLINTE/releases/download/v1.0.0/RCV-Client-1.0.0.jar)** and place it in your Minecraft `mods` folder.
5. Launch the **Fabric 1.21.11** profile and open the RCV Client menu.

> [!IMPORTANT]
> If you previously installed the original Remix fork, **remove its JAR from the same `mods` folder first** to avoid duplicate-mod conflicts. Existing configuration paths have intentionally been preserved for compatibility.

<details>
<summary><b>📂 Where is the mods folder?</b></summary>

| System | Standard Minecraft directory |
|:--|:--|
| **Windows** | `%appdata%\.minecraft\mods` |
| **Linux** | `~/.minecraft/mods` |
| **macOS** | `~/Library/Application Support/minecraft/mods` |

Custom launchers can use a different game directory. In that case, open the directory configured in your launcher.

</details>

## 🧩 Compatibility

| Requirement | Supported / recommended |
|:--|:--|
| **Minecraft** | Java Edition **1.21.11** |
| **Mod loader** | **Fabric**, tested for build configuration with Loader **0.19.3** |
| **Java runtime** | **Java 21** |
| **Fabric API** | Required; choose the Minecraft **1.21.11** build |
| **Platform** | Desktop Java; **Windows recommended** for included JavaFX music components |
| **Android / Zalith** | **Not verified**; JavaFX Windows components may not work |

> [!WARNING]
> **v1.0.0 is a beta release.** The JAR compiles successfully and passed archive-integrity checks, but it has **not yet completed real-device gameplay testing**. Please report issues you encounter.

## 🚀 What's improved in v1.0.0?

| Area | Update |
|:--|:--|
| 💜 **Appearance** | Purple visual identity for the main menu, panels, buttons, HUD defaults and music screens |
| 🏷️ **Branding** | RCV Client v1.0.0 title and version indicators |
| 🌍 **Official site** | RCV-MC.BOND button in the main menu |
| 🖼️ **Main menu** | Removed duplicate button rendering |
| 📊 **HUD / TabGUI** | Cached category module lists to reduce allocations |
| 🎨 **Color picker** | Reduced gradient rendering to 48 strips |
| 🪟 **Window title** | Avoid repeated native title changes every tick |
| 🌙 **Background performance** | Respect Minecraft's inactive-window FPS limiter |
| 🧹 **Compatibility cleanup** | Removed an unused legacy mixin accessor |

All original gameplay module implementations remain unchanged by this RCV customization.

## ❓ Frequently asked questions

<details>
<summary><b>Does RCV Client guarantee higher FPS?</b></summary>

No. It includes targeted rendering and UI optimizations, but actual FPS improvements have not been benchmarked on specific hardware. For best results, tune Minecraft graphics settings and disable modules you do not use.

</details>

<details>
<summary><b>Can I use it on my phone with Zalith Launcher?</b></summary>

It may require additional compatibility work. **Android use has not been verified**, particularly the JavaFX music components bundled for Windows.

</details>

<details>
<summary><b>Why does the internal Fabric mod ID differ from the RCV name?</b></summary>

The original internal mod ID and configuration paths are retained to avoid unnecessarily breaking existing client configurations. The displayed name is **RCV Client**, version **1.0.0**.

</details>

<details>
<summary><b>Can I use gameplay modules on multiplayer servers?</b></summary>

Only where the server's rules allow them. RCV Client is intended for use in environments where the operator permits the relevant functionality.

</details>

<details>
<summary><b>Is this a stable release?</b></summary>

This is the initial **beta**. Its source compiled with Gradle and the distributable JAR passed archive-integrity verification. Gameplay stability must still be tested on your target system.

</details>

## 🌍 دليل سريع بالعربي

<details>
<summary><b>افتح شرح تحميل وتشغيل RCV Client بالعربي</b></summary>

**RCV Client 1.0.0** مخصص لـ **Minecraft Java 1.21.11** ويشتغل على **Fabric**.

1. نزّل Minecraft Java **1.21.11** وثبّت **Fabric Loader**.
2. نزّل **Fabric API** المتوافق ويا نفس إصدار ماين كرافت.
3. حمّل **[RCV-Client-1.0.0.jar](https://github.com/CJ-RCV/RCV-CLINTE/releases/download/v1.0.0/RCV-Client-1.0.0.jar)**.
4. انقل الملف إلى مجلد **mods** وشغّل اللعبة من بروفايل Fabric.

> **مهم:** لا تجمع ملف Remix الأصلي وملف RCV بنفس مجلد المودات. والنسخة حالياً تجريبية، ودعم Android بعده مو مؤكد.

**الموقع الرسمي:** [RCV-MC.BOND](https://rcv-mc.bond)

</details>

## 📡 Support & links

<div align="center">

| Official RCV site | Releases | Issues & feedback |
|:--:|:--:|:--:|
| **[RCV-MC.BOND](https://rcv-mc.bond)** | **[All versions](https://github.com/CJ-RCV/RCV-CLINTE/releases)** | **[Report a problem](https://github.com/CJ-RCV/RCV-CLINTE/issues/new)** |

**RCV Client — Version 1.0.0 · Minecraft Java 1.21.11**

*Built for players who want a more personalized Minecraft experience.*

</div>

---

<div align="center">
<sub>Based on <a href="https://github.com/Slingerspir/Remix-1.21.11-fork-by-Sling">Remix</a> © 2026 Remix · RCV modifications © 2026 RCV · MIT License (notice included in the JAR) · Third-party assets may have separate terms.</sub>
</div>
