# Contributing to RisingV

First, thank you for considering a contribution! We welcome issues, feature proposals, and pull‑requests. To keep the code‑base healthy and the community respectful, please follow the guidelines below.

---

## Workflow

| Step | Action                                                                                          |
| ---- |-------------------------------------------------------------------------------------------------|
| 1    | **Fork** the repository and create a topic branch from `dev` (`feature/xyz`, `fix/abc`, etc.).  |
| 2    | **Write code & tests**, following the coding‑style rules below.                                 |
| 3    | Run **`dotnet test`** and **`dotnet format`** (or `dotnet format verify`) locally.              |
| 4    | Commit with a clear, present‑tense **commit message** (e.g. `fix(config): ignore missing key`). |
| 5    | **Push** your branch and open a **Pull Request (PR)** against `dev`.                            |
| 6    | At least **one maintainer review is required**. Address any review comments.                    |
| 7    | The maintainer team merges with a **squash commit**.                                            |

> **Note** – Draft PRs are absolutely fine while you are still working. They trigger CI but signal that the code isn’t ready for review.

---

## Code‑Style Requirements

### 1. Languages in this Project

* **C# 11 / .NET 8+** (primary)
* JSON & simple text assets

### 2. C# Conventions (derived from existing code)

| Category            | Rule                                                                                                                                                                                                                                    |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Indentation**     | 4 **spaces**, no tabs.                                                                                                                                                                                                                  |
| **Braces**          | *K\&R* — opening brace on **same line** as declaration (`class Foo {`).                                                                                                                                                                 |
| **Namespaces**      | `namespace Foo.Bar;` file‑scope syntax preferred.                                                                                                                                                                                       |
| **Naming**          | <ul><li>**PascalCase** for *public* types, methods, properties.</li><li>**camelCase** for local vars & private fields.</li><li>Prefix private readonly fields with `_` only when needed for clarity (match surrounding code).</li></ul> |
| **Modifiers order** | `public static async Task` (access ➜ static ➜ async ➜ type).                                                                                                                                                                            |
| **`var` usage**     | Allowed when the type is obvious from the right‑hand side; otherwise spell it out.                                                                                                                                                      |
| **XML docs**        | Every public symbol **must** have an XML summary (`///`).                                                                                                                                                                               |
| **File headers**    | Keep the SPDX & copyright header at the top (see existing files).                                                                                                                                                                       |
| **Analyzers**       | The solution ships with Roslyn analyzers — build **must be warning‑clean**.                                                                                                                                                             |
| **Nullable**        | `#nullable enable` is on; handle nullability warnings.                                                                                                                                                                                  |

> Run `dotnet format` before committing; CI fails if formatting/analyzer warnings are introduced.

### 3. JSON & Text Assets

* Use 2‑space indent in JSON.
* Keys in **camelCase**.

---

## 🔍 Tests & CI

* Add/extend **unit tests** in the `Tests/` folder.
* All PRs run the **GitHub Actions** workflow: restore → build → `dotnet test` → `dotnet format --verify`.
* A red build blocks merge.

---

## 🤝 Code of Conduct

We follow the [Contributor Covenant v2.1](https://www.contributor-covenant.org/version/2/1/code_of_conduct/). In short:

* **Be respectful.** No harassment, discrimination, or personal attacks.
* **Focus on code & ideas, not individuals.**
* If you see unacceptable behavior report it privately to the maintainers.

---

## 💬 Getting Help

* **Issues → Q\&A** — search first, then open a new issue if your question isn’t answered.
* Join the project’s Discord channel (link in the README) for synchronous discussion.

---

Thank you for helping make RisingV better!
