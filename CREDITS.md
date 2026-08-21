# Credit and attribution

## Playnite

OmniPlay is a fork of **[Playnite](https://github.com/JosefNemec/Playnite) 10.56** by
**Josef Nemec**, used under the **MIT licence**.

That is not a footnote. The library model, the plugin SDK, the theme system, the emulation support,
the fullscreen mode and the translation work of dozens of people all came from that project. What
OmniPlay adds — a 64-bit .NET 10 runtime, the mod-tool injection, the credential-free store
scanners, the folder scanner, the discovery surfaces and a new default interface — sits on roughly a
decade of somebody else's work.

The MIT copyright notice travels with the code and is meant to stay that way.

> Copyright (c) 2020 Josef Nemec
>
> Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
> associated documentation files (the "Software"), to deal in the Software without restriction …

Playnite is a **separate, actively developed project**. Its maintainers have never seen this code
and cannot support it. Please do not send them OmniPlay problems.

## The tools OmniPlay installs

OmniPlay does not bundle these. It fetches each one from its own official release feed at the moment
you ask for it, so what you get is the current version and it comes from the people who make it.

- **[ReShade](https://reshade.me)** by Patrick Mours
- **[Special K](https://special-k.info)** by Andon M. Coleman (Kaldaien)
- **[DXVK](https://github.com/doitsujin/dxvk)** by Philip Rebohle and contributors

They are separate projects under their own licences and are not affiliated with OmniPlay.

## Data

- The **emulation ROM database** (108 platforms) is derived from the
  [libretro database](https://github.com/libretro/libretro-database) and is redistributed as
  Playnite ships it.
- Game metadata comes from the provider you choose: IGDB, SteamGridDB, PCGamingWiki, IGN, GOG,
  Xbox, PSN and Steam. Each is that provider's data under that provider's terms.
- Price data comes from **[IsThereAnyDeal](https://isthereanydeal.com)**, with your own API key.
- Cover art, logos and trailers belong to the publishers and developers of the games they depict.

## Libraries

Chromium Embedded Framework via **CefSharp** · **LiteDB** · **Magick.NET** ·
**PhotoSauce.MagicScaler** · **Microsoft.PowerShell.SDK** · **NLog** · **Newtonsoft.Json** ·
**YamlDotNet** · **Markdig** · **AngleSharp** · **HtmlRenderer.WPF** · **Flurl** · **Polly** ·
**Nett** · **CommandLineParser** · **Crc32.NET** · **PdfSharp** · **VirtualizingWrapPanel** ·
**Hardcodet.NotifyIcon.Wpf** · **Microsoft.Xaml.Behaviors.Wpf** · **System.IO.Abstractions**

Every one of them ships with its own licence text in the installed application.

## Typefaces

- **[Space Grotesk](https://floriankarsten.github.io/space-grotesk/)** by Florian Karsten, SIL Open
  Font Licence 1.1 — shipped with the app.
- **Cascadia Mono** by Microsoft, SIL Open Font Licence 1.1 — used where present on the system.

## Trademarks

Steam, Epic Games, GOG, Battle.net, EA, Ubisoft Connect, Xbox, Amazon Games and Rockstar Games are
trademarks of their respective owners. OmniPlay is not affiliated with, endorsed by, or sponsored by
any of them; it reads what their clients have already written to your own disk.
