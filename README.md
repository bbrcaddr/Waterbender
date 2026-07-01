<!--
  This is the README for the PUBLIC distribution repo (github.com/bbrcaddr/Waterbender):
  binaries + issues + releases, no source. Copy it to that repo's README.md.
  (The build-from-source README stays in the private dev repo.)
-->

# Waterbender

**A visual application builder — design real desktop apps and websites, no boilerplate.**

Waterbender is a cross‑platform desktop tool for building applications
_visually_ — **free for non‑commercial use**. Lay out multi‑window UIs on a
canvas, wire up behavior with visual
**blueprints** (a node graph that compiles to JavaScript) or drop into full‑JS
mode with the [`@waterbender-app/sdk`](https://github.com/bbrcaddr/waterbender-sdk),
preview it live, and ship it as a **native desktop app** or a **self‑contained
static website**.

<!-- Add a hero screenshot / GIF here -->
<!-- ![Waterbender editor](docs/screenshots/editor.png) -->

- ⬇️ **[Download the latest release](https://github.com/bbrcaddr/Waterbender/releases/latest)** (Windows · macOS · Linux)
- 🐛 **[Report a bug or request a feature](https://github.com/bbrcaddr/Waterbender/issues)**
- 🧩 **[Full‑JS SDK](https://github.com/bbrcaddr/waterbender-sdk)** — `npm install @waterbender-app/sdk`

---

## Why Waterbender?

Most tools make you choose between two bad options:

- **Hand‑coding** a UI framework — powerful, but slow to start and full of
  boilerplate, build config, and glue code before you draw a single button.
- **No‑code builders** — fast to start, but they lock you into their platform
  and hosting, and you can rarely export a _real_, portable application.

Waterbender sits in between and refuses that trade‑off:

- **You own the output.** Export a plain **HTML/CSS/JS website** that runs
  anywhere, or a **native binary** — no runtime lock‑in, no mandatory hosting,
  no account required.
- **No ceiling.** Blueprints get you moving fast; when you need more, the
  **same runtime** is available as a typed JavaScript SDK, so you can mix visual
  and hand‑written logic freely. What you build in blueprints and what you write
  in code share one reactive state store.
- **Small and fast.** Built on [Tauri](https://tauri.app) (Rust + the system
  webview), so the apps are lightweight — not multi‑hundred‑MB Electron bundles.
- **Free for non‑commercial use** (a paid plan for commercial use is on the
  way), and it auto‑updates itself.

## Features

- Visual canvas with multiple windows/pages, drag‑drop, nesting, and a broad
  component library (buttons, inputs, sliders, switches, media, containers,
  progress bars, and more).
- **Blueprints** — connect _events → logic → actions_ visually; they compile to
  readable JavaScript.
- **Full‑JS mode** — hook app state, components, and events from plain JS via the
  SDK.
- **Live preview** and multi‑page navigation.
- **Export targets** — native desktop app _or_ a static website.
- Per‑window **theming** (system / dark / light).
- **Automatic updates.**

## Download & install

Grab the installer for your platform from the
**[Releases page](https://github.com/bbrcaddr/Waterbender/releases/latest)**:

| Platform    | File                               | Notes                                    |
| ----------- | ---------------------------------- | ---------------------------------------- |
| **Windows** | `Waterbender_x.y.z_x64-setup.exe`  | NSIS installer (64‑bit).                 |
| **macOS**   | `Waterbender_x.y.z_universal.dmg`  | Universal — Apple Silicon **and** Intel. |
| **Linux**   | `waterbender_x.y.z_amd64.AppImage` | `chmod +x` it, then run.                 |

### First‑launch security prompt (one time)

The public builds are **not code‑signed** (that keeps them free), so your OS
shows a one‑time "unrecognized app" warning on the **first** launch. This is
expected; here's how to proceed:

- **Windows** — SmartScreen → **More info** → **Run anyway**.
- **macOS** — **right‑click the app → Open** (then confirm), or run
  `xattr -dr com.apple.quarantine /Applications/Waterbender.app`.
- **Linux** — no prompt; just make the AppImage executable.

After the first launch, **updates are seamless** — the in‑app updater downloads
new versions directly, with no further warnings.

## Releases

- Every release is tagged **`vX.Y.Z`** on the
  [Releases page](https://github.com/bbrcaddr/Waterbender/releases) and includes
  installers for all three platforms plus release notes describing what changed.
- Versioning follows **[SemVer](https://semver.org)** — `MAJOR.MINOR.PATCH`.
- **Auto‑update:** Waterbender checks for a newer release on startup; if one
  exists it offers to download, install, and relaunch. You can always grab a
  build manually from the Releases page instead.

## Reporting bugs & requesting features

Bug reports and feature requests go through
**[GitHub Issues](https://github.com/bbrcaddr/Waterbender/issues)**.

**Before opening one:** please
[search existing issues](https://github.com/bbrcaddr/Waterbender/issues?q=is%3Aissue)
in case it's already reported — a 👍 on an existing issue helps prioritize it.

**A good bug report includes:**

1. **Waterbender version** (and how you installed it) and **your OS + version**
   (e.g. Windows 11, macOS 14 (Apple Silicon), Ubuntu 24.04).
2. **Steps to reproduce** — the shorter and more exact, the better.
3. **What you expected** vs. **what actually happened.**
4. **Screenshots or a short screen recording** for anything visual.
5. If you can, a **minimal `.wb` project** that reproduces it (or the relevant
   blueprint/script), and any **error output** from the console.

Clear, reproducible reports get fixed fastest. For feature requests, describe the
problem you're trying to solve, not just the solution you have in mind.

> **Security issues:** please **don't** open a public issue for anything
> exploitable — report it privately (see `SECURITY.md`) so it can be fixed before
> disclosure.

## Source & contributing

Waterbender ships as pre‑built binaries; the editor's source is not public. The
**SDK is open source** — if you build in full‑JS mode, contributions and issues
are welcome at
[bbrcaddr/waterbender-sdk](https://github.com/bbrcaddr/waterbender-sdk). For the
app itself, the best way to help is a good **bug report** or **feature request**.

## License & pricing

- **Non‑commercial use is free.** Personal, educational, and other
  non‑commercial use of Waterbender is free of charge.
- **Commercial use requires a paid plan.** Using Waterbender in a business or to
  build/ship software for commercial purposes needs a paid commercial license.
  A paid plan is **in development** — for now only the free build is available;
  reach out about commercial licensing in the meantime.
- **Your work is yours.** You own the projects and the apps/websites you export.

See [`LICENSE`](LICENSE) for the full terms. The companion
[`@waterbender-app/sdk`](https://github.com/bbrcaddr/waterbender-sdk) is separate
and **MIT‑licensed**.
