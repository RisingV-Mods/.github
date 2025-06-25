# RisingV

A V Rising modding framework built for BepInEx by [BenDol](https://github.com/BenDol).

![Your GitHub Stats](https://github-readme-stats.vercel.app/api?username=BenDol&show_icons=true&theme=dark)

Welcome to the RisingV GitHub. My mission is to provide a suite of modular libraries, tools, and systems that enhance the V Rising modding experience, making it easier to create immersive gameplay, custom mechanics, and advanced features for your mods.

---

## Table of Contents

* [Projects](#projects)
* [Documentation](#documentation)
* [Concerns](#concerns)
* [Community](#community)
* [Getting Started](#getting-started)
* [Contributing](#contributing)
* [License](#license)

---

## Projects

Below is a list of my core repositories. Each is designed to be used independently or together as building blocks for your V Rising mods:

|      | Name | Type | Description |
|:----:|:----:|:----:|:------------|
| [![](https://github.com/RisingV-Mods/RisingV.Shared/blob/main/assets/images/logo_50.png?raw=true)](https://github.com/RisingV-Mods/RisingV.Shared) | [RisingV.Shared](https://github.com/RisingV-Mods/RisingV.Shared) | Lib | Contains shared libraries, helper functions, and common data structures used across multiple RisingV projects. Ideal for dragging into any mod that needs reusable assets or utilities. [API Docs](https://docs.risingv.dev/shared/api/RisingV.Shared.html) |
| [![](https://github.com/RisingV-Mods/RisingV.Core/blob/main/assets/images/logo_50.png?raw=true)](https://github.com/RisingV-Mods/RisingV.Core) | [RisingV.Core](https://github.com/RisingV-Mods/RisingV.Core) | Lib | Provides essential systems and utilities—such as data management, event handling, and configuration services—that form the backbone of many mods. [API Docs](https://docs.risingv.dev/core/api/RisingV.Core.html) | Lib |
| [![](https://github.com/RisingV-Mods/RisingV.Scripting/blob/main/assets/images/logo_50.png?raw=true)](https://github.com/RisingV-Mods/RisingV.Scripting) | [RisingV.Scripting](https://github.com/RisingV-Mods/RisingV.Scripting) | Lib | Exposes a scripting API that lets you write C# scripts executing at runtime. Includes a runtime host to load and manage scripts without recompiling the entire mod. [API Docs](https://docs.risingv.dev/scripting/api/RisingV.Scripting.html) |
| [![](https://github.com/RisingV-Mods/RisingV.GameData/blob/main/assets/images/logo_50.png?raw=true)](https://github.com/RisingV-Mods/RisingV.GameData) | [RisingV.GameData](https://github.com/RisingV-Mods/RisingV.GameData) | Lib | A data pack library with V Rising specific data (internally used by RisingV.Core so not required as a seperate dependency, but can be used this way in your mod if you require). [GitHub Repo](https://github.com/BenDol/RisingV.GameData) |
| [![](https://github.com/RisingV-Mods/RisingV.BossDrops/blob/main/assets/images/logo_50.png?raw=true)](https://github.com/RisingV-Mods/RisingV.BossDrops) | [RisingV.BossDrops](https://github.com/RisingV-Mods/RisingV.BossDrops) | Mod | A mod that demonstrates advanced usage of RisingV libraries by extending V Rising’s boss drop system. Use it as a template or reference when creating your own drop modifications. [GitHub Repo](https://github.com/BenDol/RisingV.BossDrops) |

## Documentation

All of my public APIs and usage guides are hosted on the docs site:

* **Main Documentation Portal**: [https://docs.risingv.dev](https://docs.risingv.dev/)
* **Getting Started Guide**: [https://docs.risingv.dev/sample](https://docs.risingv.dev/sample)
* **API References**: _(See table above)_

Be sure to visit the site for examples, tutorials, and up-to-date changelogs.

## Concerns

**Game Updates**  
One of RisingV's goals is to make sure that game updates have as little friction as possible by modularizing components where possible. Below is a diagram that demonstrates which libraries are affected by game updates (red = affected, green = immune). This will be updated as required. Stability is a very important factor in my development process and I want to make sure RisingV doesn't cause more issues than it solves.

![RisingV_Game_Updates drawio](https://github.com/user-attachments/assets/7e542a5f-2da9-43b2-9baf-ce76f9c144e8)

## Community

Join the community to get help, share your work, and collaborate with other modders:

* **Discord**: [https://vrisingmods.com/discord](https://vrisingmods.com/discord) (VRising Mod Community)
* **Twitter (X)**: [https://twitter.com/RisingVModding](https://twitter.com/RisingVMods)
* **Issues & Discussions**:

  * File bugs, request features, or discuss usage on each repository’s “Issues” tab.
  * General conversation and announcements take place in my GitHub Discussions (where available).

## Getting Started

For detailed, step-by-step instructions, see the [Getting Started](https://docs.risingv.dev/sample) section in the documentation.

## Contributing

We welcome contributions of all kinds—bug fixes, documentation improvements, new features, and sample mods. To participate:

1. Fork the repo you want to work on (e.g., [RisingV.Core](https://github.com/RisingV-Mods/RisingV.Core)).
2. Create a new branch for your feature or fix.
3. Follow existing coding conventions and add comments where necessary.
4. Submit a pull request describing your change.

Please see each repository’s `CONTRIBUTING.md` for specific guidelines and coding standards. If you’re unsure where to start, check out open issues labeled **good first issue**.

## License

All RisingV repositories are licensed under the **MIT License**. By using or contributing to RisingV, you agree to the terms of this license. For details, see [LICENSE](https://github.com/BenDol/RisingV.Core/blob/main/LICENSE).

---

Thank you for checking out RisingV! I look forward to seeing what you create.
