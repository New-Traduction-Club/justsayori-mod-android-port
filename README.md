# JSL: An After Story Launcher (Official Android Port)

<!-- [![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)]()
[![Platform](https://img.shields.io/badge/platform-Android-blue.svg)]()
[![License](https://img.shields.io/badge/license-Custom-orange.svg)]() -->

> **STRICT DISCLAIMER & IMPORTANT NOTICE**
> 1. **NO ASSETS INCLUDED:** This repository does **not** contain any game assets, artwork, or music from *Doki Doki Literature Club!* (DDLC).
> 2. **SCOPE:** This repository solely contains the Android project structure, the Ren'Py engine wrapper, and custom tools designed to facilitate the execution of legally obtained mod files on Android devices.

---

## Overview

**JSL (An After Story Launcher)** is a custom Android port designed to run the *Just Sayori* mod seamlessly on mobile environments. Built upon a highly customized fork of Ren'Py's RAPT (Ren'Py Android Packaging Tool), JSL provides a native-like experience with advanced features specifically tailored for the JS community.

## Key Features

- **One-Click Installation:** Automatic download and setup of the JS mod.
- **Content Installers:** Built-in managers for **Spritepacks** and **Submods**.
- **Discord Rich Presence:** Using integrated [KizzyRPC](https://github.com/KizzyRPC). (Still working on that lol)
- **File Explorer:** Integrated file manager to handle game files, submods, etc.
- **Multi-Language Support:** Fully localized in English, Español, and Português.
- **Optimized Engine:** Custom Kotlin-based `unrpa` implementation and stockfish 8 library.
- **Cool UI:** A launcher based in another cool UI...

## Installation

To use JSL, you must provide your own legally obtained copy of DDLC and the Just Sayori mod.

1. **Download DDLC:** Obtain the Windows version of Doki Doki Literature Club from [ddlc.moe](https://ddlc.moe/).
2. **Download JS:** Obtain the latest version of Just Sayori from the [official GitHub](https://github.com/New-Traduction-Club/justsayori-mod/releases).
3. **Run JSL:** Launch the app on your Android device and follow the step-by-step setup guide:
   - Select your DDLC `.zip` file.
   - Select your JS `.zip` file (or use the "Automatic Download" option).
   - Let JSL verify, extract, and configure the game for you.

## Components
- **Kotlin Integration:** Native Android components handle heavy lifting like ZIP extraction, RPA unpacking, Discord RPC, notifications, etc.
- **Internal Storage Provider:** A custom DocumentsProvider to allow external apps to interact with game files securely.

### The `unrpa` Kotlin Implementation
To handle Ren'Py Archive (`.rpa`) extraction natively, we developed a custom `unrpa` utility in Kotlin.
* **Logic Attribution:** Based on the Python implementation by [Lattyware](https://github.com/Lattyware/unrpa).

## Development

### Prerequisites
- JDK 17+.
- Android SDK 34+.

### Building from Source
```bash
./gradlew assembleDebug
```

## Credits

*   **[Team Salvato](https://teamsalvato.com/):** For creating the incredible *Doki Doki Literature Club!*
*   **[Monika After Story Team](https://www.monikaafterstory.com/):** For the original mod and their continuous hard work.
*   **[Ren'Py](https://www.renpy.org/):** For the visual novel engine.
*   **[KizzyRPC](https://github.com/KizzyRPC):** For the Android Discord RPC implementation.

---
*Developed and maintained by Traduction Club!*
