<p align="center">
  <!-- Animated: tiles light up in a diagonal wave, the way a library fills in. The still
       1600x500 version stays in assets/brand for anywhere a GIF is the wrong answer. -->
  <img src="assets/brand/banner.gif?v=20260822-premium-motion-v3" alt="OmniPlay — Every game you own. One library, built-in tools." width="100%">
</p>

<h1 align="center">OmniPlay</h1>
<p align="center"><b>Every game you own, in one place — and the tools you run them with.</b></p>
<p align="center">Part of the <a href="#the-omnivex-suite">OmniVex</a> suite.</p>

<p align="center">
  <a href="https://www.patreon.com/TheOmniGrid"><img alt="Get it on Patreon" src="https://img.shields.io/badge/Get%20it%20on-Patreon-FF424D?style=for-the-badge&logo=patreon&logoColor=white"></a>
  &nbsp;
  <a href="https://ko-fi.com/theomnigrid"><img alt="Get it on Ko-fi" src="https://img.shields.io/badge/Get%20it%20on-Ko--fi-FF5E5B?style=for-the-badge&logo=kofi&logoColor=white"></a>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/version-1.0.0.0-8A7BFF?style=flat-square">
  <img alt="Platform" src="https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20x64-0078D4?style=flat-square&logo=windows&logoColor=white">
  <img alt="Languages" src="https://img.shields.io/badge/languages-45-8A7BFF?style=flat-square">
  <img alt="Telemetry" src="https://img.shields.io/badge/telemetry-none-2EA043?style=flat-square">
  <img alt="License" src="https://img.shields.io/badge/license-MIT-6A5BDB?style=flat-square">
</p>

<!-- Quick navigation. Each chip links to a section of this page or to the document it names. The anchors
     are GitHub's own slugs for the headings below - rename a heading and its chip has to be
     renamed with it. -->
<p align="center">
  <a href="#get-omniplay"><img alt="Get OmniPlay" src="https://img.shields.io/badge/⬇%20Get%20OmniPlay-8A7BFF?style=for-the-badge"></a>
  <a href="#what-it-does"><img alt="Features" src="https://img.shields.io/badge/Features-2B2545?style=for-the-badge"></a>
  <a href="#the-mod-tools-are-the-point"><img alt="Mod tools" src="https://img.shields.io/badge/Mod%20tools-2B2545?style=for-the-badge"></a>
  <a href="#a-game-page-not-a-spreadsheet"><img alt="Screenshots" src="https://img.shields.io/badge/Screenshots-2B2545?style=for-the-badge"></a>
  <a href="#privacy"><img alt="Privacy" src="https://img.shields.io/badge/Privacy-2B2545?style=for-the-badge"></a>
  <a href="#compatibility-with-playnite"><img alt="Compatibility" src="https://img.shields.io/badge/Compatibility-2B2545?style=for-the-badge"></a>
  <a href="FAQ.md"><img alt="FAQ" src="https://img.shields.io/badge/FAQ-2B2545?style=for-the-badge"></a>
  <a href="SUPPORT.md"><img alt="Support" src="https://img.shields.io/badge/Support-2B2545?style=for-the-badge"></a>
  <a href="CHANGELOG.md"><img alt="Changelog" src="https://img.shields.io/badge/Changelog-2B2545?style=for-the-badge"></a>
</p>

> [!IMPORTANT]
> **Documentation-only repository.** This public repository contains OmniPlay documentation, approved artwork, and screenshots—not the application source tree, installer, binary releases, signing material, or private build infrastructure. Official distribution remains outside GitHub.

<p align="center">
  <img src="assets/screenshots/library.jpg" alt="The OmniPlay library" width="920">
</p>

---

## What it is

OmniPlay finds the games you already have — across Steam, Epic, GOG, Battle.net, EA, Ubisoft, Xbox,
Amazon, Rockstar, emulators, and plain folders on a drive — and puts them in one library. Then it
does the part a launcher usually leaves to you: it installs and tracks **ReShade, Special K and
DXVK** per game, and tells you what each game already has.

It is a fork of [Playnite](https://github.com/JosefNemec/Playnite) by Josef Nemec, rebuilt on
**.NET 10, 64-bit**, with the jobs that mattered most built in rather than bolted on.

> **OmniPlay is donationware.** Free, complete, no ads, no paid tier, nothing held back. There is
> no public download yet — supporters get the build first. See [Get OmniPlay](#get-omniplay).

---

## What it does

|  | |
|---|---|
| **Mod and graphics tools per game** | ReShade, Special K and DXVK installed into a game's folder from inside OmniPlay, with a badge in the library for what each game already carries. |
| **Store scanning without signing in** | Eight store clients read from their own local manifests. No login, no token, no session cookie. |
| **Every launcher in one library** | The nine upstream library plugins are bundled too, for the extras only a signed-in account can give you. |
| **A folder scanner** | Point it at `X:\Games\` and games installed outside any launcher become first-class library entries. |
| **A discovery layer** | Store catalogue search, current deals, a wishlist with price alerts, and a release calendar. |
| **Emulation that can name a ROM** | The 108-platform ROM database that upstream packages outside its source tree, and that source builds therefore never had. |
| **Metadata from ten providers** | IGDB, SteamGridDB, PCGamingWiki, IGN, GOG, Xbox, PSN, Steam, Steam Tags, and local files. |
| **Fullscreen mode** | Including the quick access menu and handheld layouts. |
| **45 languages** | Inherited from a decade of upstream translation work. |

---

## The mod tools are the point

Every other launcher stops at "here is your game". OmniPlay knows what is *inside* the game folder.

<p align="center">
  <img src="assets/screenshots/game-mods.jpg" alt="The Mods tab on a game page" width="100%">
</p>

The library badge can only say yes or no. The game page's **Mods** tab says which tool, which
version, and which file name it loads under — the answer you need when two tools want the same
proxy DLL.

Versions are resolved from each tool's **own release feed at the moment you install**, never pinned
to whatever was current when the build was made. DXVK is refused for games that do not use Direct3D
8–11, and refused alongside ReShade or Special K, because it replaces Direct3D rather than layering
on top of it — with the reason on the greyed-out row instead of a silent failure.

---

## A game page, not a spreadsheet

<p align="center">
  <img src="assets/screenshots/game-overview.jpg" alt="A game page in OmniPlay" width="100%">
</p>

Key art as the page's own backdrop, the trailer playing in the same place if the game has one, and
three tabs instead of one endless scroll: **Overview** for the four numbers you actually came for,
**Details** for the other twenty-one fields and every link, **Mods** for what is installed.

<p align="center">
  <img src="assets/screenshots/game-details.jpg" alt="The Details tab" width="100%">
</p>

---

## Privacy

Your library lives on your PC. **No telemetry, no usage reporting, no account, no crash upload.**

Playnite's crash handler uploads a diagnostics package to its own server. OmniPlay writes the package
next to you and opens the folder instead — your logs stay on your machine.

OmniPlay contacts the network only when a feature you used needs it: a metadata provider you asked
to download from, a store plugin you enabled, the add-on index when you browse add-ons, the release
feed of a graphics tool at the moment you install it, and the discovery surfaces if you gave them
keys.

Those keys are **yours**. The catalogue reads IGDB and the prices read IsThereAnyDeal; both are free
and both need an account of your own. They are stored in **Windows Credential Manager**, never in a
settings file. OmniPlay ships no keys of its own, and those surfaces do nothing until you add yours.

See [PRIVACY.md](PRIVACY.md).

---

## Compatibility with Playnite

OmniPlay keeps its library in `%AppData%\OmniPlay` and its program files in `%LocalAppData%\OmniPlay`.
Playnite's own `%AppData%\Playnite` is **never read and never written**. Both programs can be
installed and run at the same time; on the development machine they are.

Your library is copied and converted on first run. The original is left alone.

Your existing **plugins and themes keep working**: the SDK assembly is still `Playnite.SDK` with
unchanged namespaces, on purpose.

---

## Get OmniPlay

**There is no public download yet.** OmniPlay is finished enough to use daily and is being used
daily — but it has not been through anyone else's hands, and a first release that has only ever run
on one machine is not a release.

Builds go to supporters first, the same way the rest of the OmniVex tools are handled:

<p align="center">
  <a href="https://www.patreon.com/TheOmniGrid"><img src="assets/brand/support-patreon.svg" height="64" alt="Support OmniPlay on Patreon"></a>
  &nbsp;&nbsp;
  <a href="https://ko-fi.com/theomnigrid"><img src="assets/brand/support-kofi.svg" height="64" alt="Support OmniPlay on Ko-fi"></a>
</p>

**Requirements:** Windows 10 or 11, 64-bit. The runtime ships with the app — no separate .NET
install.

This repository is the project's front page. **The source code and the installer are not here**, and
that is deliberate.

---

## Documentation

| | |
|---|---|
| [Privacy](PRIVACY.md) | Local data, third-party libraries and telemetry boundaries |
| [FAQ](FAQ.md) | Availability, compatibility and common product questions |
| [Support](SUPPORT.md) | Useful reports, privacy redaction and contact routes |
| [Security](SECURITY.md) | Private vulnerability reporting |
| [Contributing](CONTRIBUTING.md) | Documentation and reproducible-report scope |
| [Changelog](CHANGELOG.md) | Public project history |
| [Licence](LICENSE.md) | Playnite lineage and application terms |
| [Credits](CREDITS.md) | Upstream project and third-party attribution |

---

## The OmniVex suite

OmniPlay is one of a family of tools sharing a design language and a philosophy —
modern, fast, no telemetry:

**OmniTheme** · **OmniBlock** · **OmniCleaner** · **OmniAPO** · **OmniEQ** · **OmniPlay** · **OmniScale** · **OmniShade** · **OmniVisuals** · **OmniGPU** · **OmniWrappers**

<sub>**OmniWrappers** is four Direct3D compatibility installers — OmniDXVK, OmniDxWrapper, OmniVKD3D and OmniVoodoo2.</sub>

<sub>Tuned for framerate, mixed for headroom, sharp to the pixel. Donationware
tools for gamers and audiophiles — audio, graphics, and a bit of privacy too.</sub>

More at [github.com/TheOmniGrid](https://github.com/TheOmniGrid).

---

## Credit

OmniPlay is a fork of **[Playnite](https://github.com/JosefNemec/Playnite) 10.56** by **Josef Nemec**,
MIT licensed, and would not exist without roughly a decade of his work and that of Playnite's
contributors and translators.

**Playnite is a separate, actively developed project. Please do not report OmniPlay problems to it** —
its maintainers have never seen this code. Its [user manual](https://playnite.link/docs/) is theirs
and still largely applies.

Full attribution in [CREDITS.md](CREDITS.md).

---

## Contact

Use public channels only for information that is safe to share. Remove usernames, local paths,
account identifiers, licence data, and other personal information from screenshots and logs.

| Channel | Use |
|---|---|
| [GitHub Issues](../../issues/new/choose) | Reproducible bugs, compatibility reports, and documentation corrections |
| [GitHub Discussions](../../discussions) | Questions, ideas, and community support |
| [Security](SECURITY.md) | Private vulnerability reporting — never use a public issue |
| [Email](mailto:omnivex@theomnigrid.biz) | Private support, delivery, or licensing questions |

Support is best-effort. See [SUPPORT.md](SUPPORT.md) and [CONTRIBUTING.md](CONTRIBUTING.md)
for repository scope and reporting guidance.

---

<p align="center">
  <strong>OmniPlay</strong><br>
  <a href="https://github.com/TheOmniGrid">The OmniGrid on GitHub</a> ·
  <a href="https://ko-fi.com/theomnigrid">Ko-fi</a> ·
  <a href="https://www.patreon.com/TheOmniGrid">Patreon</a><br><br>
  <sub>Copyright © 2026 OmniVex · MIT licensed · <a href="LICENSE.md">Legal &amp; licensing</a></sub><br>
  <sub>A fork of Playnite © Josef Nemec and contributors, used under the MIT licence. Steam, Epic, GOG, Battle.net, EA, Ubisoft, Xbox, Amazon and Rockstar are trademarks of their respective owners; OmniPlay is not affiliated with them.</sub>
</p>
