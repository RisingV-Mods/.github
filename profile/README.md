# RisingV

A V Rising modding framework built for BepInEx by [BenDol](https://github.com/BenDol).

![Your GitHub Stats](https://github-readme-stats.vercel.app/api?username=BenDol&show_icons=true&theme=dark)

Welcome to the RisingV GitHub. My mission is to provide a suite of modular libraries, tools, and systems that enhance the V Rising modding experience—making it easier to create immersive gameplay, custom mechanics, and advanced features for your mods.

---

## Table of Contents

* [Projects](#projects)
* [Documentation](#documentation)
* [Community](#community)
* [Getting Started](#getting-started)
* [Contributing](#contributing)
* [License](#license)

---

## Projects

Below is a list of my core repositories. Each is designed to be used independently or together as building blocks for your V Rising mods:

* **[RisingV.Core](https://github.com/RisingV-Mods/RisingV.Core)**
  Provides essential systems and utilities—such as data management, event handling, and configuration services—that form the backbone of many mods.
  [API Docs](https://docs.risingv.dev/core/api/RisingV.Core.html) ([risingv.dev][1])

* **[RisingV.Shared](https://github.com/RisingV-Mods/RisingV.Shared)**
  Contains shared libraries, helper functions, and common data structures used across multiple RisingV projects. Ideal for dragging into any mod that needs reusable assets or utilities.
  [API Docs](https://docs.risingv.dev/shared/api/RisingV.Shared.html)

* **[RisingV.Scripting](https://github.com/RisingV-Mods/RisingV.Scripting)**
  Exposes a scripting API that lets you write C# scripts executing at runtime. Includes a runtime host to load and manage scripts without recompiling the entire mod.
  [API Docs](https://docs.risingv.dev/scripting/api/RisingV.Scripting.html)

* **[RisingV.BossDrops](https://github.com/RisingV-Mods/RisingV.BossDrops)**
  An example mod that demonstrates advanced usage of RisingV libraries by extending V Rising’s boss drop system. Use it as a template or reference when creating your own drop modifications.
  [GitHub Repo](https://github.com/BenDol/RisingV.BossDrops)

---

## Documentation

All of my public APIs and usage guides are hosted on the docs site:

* **Main Documentation Portal**: [https://docs.risingv.dev/](https://docs.risingv.dev/)
* **Getting Started Guide**: [https://docs.risingv.dev/sample](https://docs.risingv.dev/sample)
* **API References**:

  * Core: [https://docs.risingv.dev/core/api/RisingV.Core.html](https://docs.risingv.dev/core/api/RisingV.Core.html)
  * Shared: [https://docs.risingv.dev/shared/api/RisingV.Shared.html](https://docs.risingv.dev/shared/api/RisingV.Shared.html)
  * Scripting: [https://docs.risingv.dev/scripting/api/RisingV.Scripting.html](https://docs.risingv.dev/scripting/api/RisingV.Scripting.html)

Be sure to visit the site for examples, tutorials, and up-to-date changelogs.

---

## Community

Join the community to get help, share your work, and collaborate with other modders:

* **Discord**: [https://vrisingmods.com/discord](https://vrisingmods.com/discord) (VRising Mod Community)
* **Twitter (X)**: [https://twitter.com/RisingVModding](https://twitter.com/RisingVMods)
* **Issues & Discussions**:

  * File bugs, request features, or discuss usage on each repository’s “Issues” tab.
  * General conversation and announcements take place in my GitHub Discussions (where available).

---

## Getting Started

1. **Clone a Base Repository**

   ```bash
   git clone https://github.com/RisingV-Mods/RisingV.Core.git
   cd RisingV.Core
   ```
2. **Install Dependencies**

   * Ensure BepInEx is installed for V Rising.
   * Add `RisingV.Shared` and `RisingV.Scripting` as project references or submodules.
3. **Review Example Mod**

   * Check out `RisingV.BossDrops` for a working example of how to wire up Core, Shared, and Scripting together.
4. **Build & Deploy**

   * Compile your project (Target .NET 4.x to match V Rising runtime).
   * Copy the resulting DLL to your V Rising `BepInEx/plugins/` folder.
   * Launch V Rising and verify your mod loads by checking the console log.

For more detailed, step-by-step instructions, see the [Getting Started](https://docs.risingv.dev/getting-started) section in the documentation.

---

## Contributing

We welcome contributions of all kinds—bug fixes, documentation improvements, new features, and sample mods. To participate:

1. Fork the repo you want to work on (e.g., [RisingV.Core](https://github.com/RisingV-Mods/RisingV.Core)).
2. Create a new branch for your feature or fix.
3. Follow existing coding conventions and add comments where necessary.
4. Submit a pull request describing your change.

Please see each repository’s `CONTRIBUTING.md` for specific guidelines and coding standards. If you’re unsure where to start, check out open issues labeled **good first issue**.

---

## License

All RisingV repositories are licensed under the **MIT License**. By using or contributing to RisingV, you agree to the terms of this license. For details, see [LICENSE](https://github.com/BenDol/RisingV.Core/blob/main/LICENSE).

---

Thank you for checking out RisingV! We look forward to seeing what you create.
