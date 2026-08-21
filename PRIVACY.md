# Privacy

**Effective date:** 21 August 2026

The short version: your library lives on your PC, OmniPlay has no account, no telemetry and no
analytics, and it never sends anything anywhere unless a feature you asked for needs it.

## What OmniPlay stores, and where

Everything is on your own machine.

| | |
|---|---|
| Library, settings, playlists, filter presets | `%AppData%\OmniPlay` |
| Program files, logs, caches | `%LocalAppData%\OmniPlay` |
| API keys you enter | **Windows Credential Manager**, under the `OmniPlay:` prefix |

Nothing is uploaded, mirrored or synchronised. There is no OmniPlay server to send it to.

**`%AppData%\Playnite` is never read and never written.** If you also run Playnite, its data is
untouched; OmniPlay converts a copy on first run and leaves the original alone.

## What is deliberately absent

- **No telemetry.** No usage counters, no feature pings, no install ID, no first-run beacon.
- **No analytics.** No third-party SDK is embedded for measurement of any kind.
- **No account.** There is nothing to sign up for.
- **No crash upload.** Playnite's crash handler uploads a diagnostics package to its own server.
  OmniPlay writes the package next to you and opens the folder. The logs inside are yours, and they
  stay yours.
- **No ads, ever**, and no paid tier that would need to know who you are.

## When OmniPlay does use the network

Only for something you asked for:

- **Metadata download** — the provider you picked, when you ask for it.
- **Store library plugins** — only the ones you enable and sign into. Those sign-ins are handled by
  each plugin against its own service; OmniPlay itself never asks you for a store password.
- **Store scanners** — these use **no network at all.** They read the manifests each launcher has
  already written to your disk.
- **Add-on browsing and update checks** — the add-on index, when you open that page.
- **Mod tools** — the release feed of ReShade, Special K or DXVK at the moment you install one.
- **Discovery surfaces** — IGDB for the catalogue and release dates, IsThereAnyDeal for prices, only
  once you have entered your own keys. Without keys those pages show sample data and make no
  requests.

## About the keys

The catalogue and the price surfaces need API keys you register yourself. They are stored in the
Windows Credential Manager — the same vault Windows uses for saved passwords — and never written
into a settings file, a log, or a diagnostics package.

OmniPlay ships no keys of its own. Nothing routes through anything belonging to OmniVex.

## Your games and cover art

Covers, logos, trailers and descriptions are downloaded to your machine from the metadata provider
you chose and cached there. What you play, when, and for how long is recorded locally so the library
can show it to you, and is not sent anywhere.

## Changes

This document is versioned with the project. Any change to what OmniPlay sends or stores gets a new
effective date at the top and a line in the release notes.

Questions: **omnivex@theomnigrid.biz**
