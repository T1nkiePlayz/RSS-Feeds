<div align="center">

# RSS Feeds

**A curated collection of RSS and Atom feeds, organised for FreshRSS.**

[All feeds](all-feeds.opml) · [Browse categories](folders/)

</div>

---

## Overview

A curated collection covering Linux, open source, programming, web development, game development, gaming, space, science, cybersecurity, technology and creative projects.

| | |
|:--|--:|
| **Feeds** | 56 |
| **Categories** | 11 |
| **Format** | OPML 2.0 |
| **Recommended reader** | [FreshRSS](https://freshrss.org/) |

## Categories

Each category has an individual OPML file. These files are designed to work with FreshRSS's **dynamic OPML category** option.

| Category | Feeds | OPML |
|:--|--:|:--|
| Linux & Open Source | 7 | [linux-open-source.opml](folders/linux-open-source.opml) |
| Programming & Software Development | 10 | [programming-software-development.opml](folders/programming-software-development.opml) |
| Web Development & Design | 6 | [web-development-design.opml](folders/web-development-design.opml) |
| Game Development | 4 | [game-development.opml](folders/game-development.opml) |
| Gaming & Minecraft | 5 | [gaming-minecraft.opml](folders/gaming-minecraft.opml) |
| Space & Science | 8 | [space-science.opml](folders/space-science.opml) |
| Cybersecurity & Privacy | 4 | [cybersecurity-privacy.opml](folders/cybersecurity-privacy.opml) |
| Technology & World News | 8 | [technology-world-news.opml](folders/technology-world-news.opml) |
| Pixel Art & Creative | 1 | [pixel-art-creative.opml](folders/pixel-art-creative.opml) |
| Self-hosting & Homelab | 1 | [self-hosting-homelab.opml](folders/self-hosting-homelab.opml) |
| Discovery & New Projects | 2 | [discovery-new-projects.opml](folders/discovery-new-projects.opml) |

## Dynamic OPML in FreshRSS

Instead of importing each file manually, you can point a FreshRSS category at its OPML URL. FreshRSS will use that remote OPML document to populate the category with its feeds.

1. Open FreshRSS and go to **Subscription management**.
2. Create a category, or open the settings for the category you want to populate.
3. Find the option for a dynamic OPML source (the field described as **“Provide the URL to an OPML file to dynamically populate this category with feeds”**).
4. Paste the matching **Raw OPML URL** from the list below.
5. Save the category. Repeat for any other categories you want.

### Raw OPML URLs

Use these URLs in FreshRSS — they point directly to the files, not to GitHub's file-preview pages.

| FreshRSS category | Raw OPML URL |
|:--|:--|
| Linux & Open Source | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/linux-open-source.opml` |
| Programming & Software Development | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/programming-software-development.opml` |
| Web Development & Design | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/web-development-design.opml` |
| Game Development | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/game-development.opml` |
| Gaming & Minecraft | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/gaming-minecraft.opml` |
| Space & Science | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/space-science.opml` |
| Cybersecurity & Privacy | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/cybersecurity-privacy.opml` |
| Technology & World News | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/technology-world-news.opml` |
| Pixel Art & Creative | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/pixel-art-creative.opml` |
| Self-hosting & Homelab | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/self-hosting-homelab.opml` |
| Discovery & New Projects | `https://raw.githubusercontent.com/T1nkiePlayz/RSS-Feeds/main/folders/discovery-new-projects.opml` |

**Important:** use the individual category OPML files for dynamic categories. The combined [`all-feeds.opml`](all-feeds.opml) is intended for a one-time full import, not as an additional source alongside all 11 dynamic categories, which could create duplicate subscriptions.

## One-time OPML import

If you prefer a normal import, download [`all-feeds.opml`](all-feeds.opml), then in FreshRSS open **Subscription management → Import / Export → Import** and upload the file.

## Repository layout

```text
RSS-Feeds/
├── README.md
├── all-feeds.opml
└── folders/
    ├── linux-open-source.opml
    ├── programming-software-development.opml
    ├── web-development-design.opml
    ├── game-development.opml
    ├── gaming-minecraft.opml
    ├── space-science.opml
    ├── cybersecurity-privacy.opml
    ├── technology-world-news.opml
    ├── pixel-art-creative.opml
    ├── self-hosting-homelab.opml
    └── discovery-new-projects.opml
```

## Community feed choices

| Previous Reddit topic | Lemmy community | Feed |
|:--|:--|:--|
| Game development | `!gamedev@programming.dev` | [RSS](https://programming.dev/feeds/c/gamedev.xml?sort=New) |
| Godot | `!godot@programming.dev` | [RSS](https://programming.dev/feeds/c/godot.xml?sort=New) |
| Minecraft | `!minecraft@lemmy.world` | [RSS](https://lemmy.world/feeds/c/minecraft.xml?sort=New) |
| Linux gaming | `!linux_gaming@lemmy.world` | [RSS](https://lemmy.world/feeds/c/linux_gaming.xml?sort=New) |
| Space | `!space@lemmy.ml` | [RSS](https://lemmy.ml/feeds/c/space.xml?sort=New) |
| Pixel art / Aseprite | `!pixelart@retrolemmy.com` | [RSS](https://retrolemmy.com/feeds/c/pixelart.xml?sort=New) |
| Self-hosting / homelab | `!selfhosted@lemmy.world` | [RSS](https://lemmy.world/feeds/c/selfhosted.xml?sort=New) |

The Aseprite and homelab topics do not currently have sufficiently active dedicated Lemmy counterparts, so they are covered by the broader pixel-art and self-hosting communities rather than by low-activity feeds.

## Maintenance

- The individual category OPML files are the sources to use for dynamic categories.
- When a category's OPML file is updated on the repository's `main` branch, its Raw URL stays the same; FreshRSS can retrieve the updated document when it refreshes that dynamic source.
- Feed availability and publisher URLs can change over time. If a publisher retires or moves a feed, the relevant OPML file will need updating.
- **Community feeds use Lemmy's native RSS:** the Reddit community subscriptions have been replaced with direct Lemmy community feeds sorted by newest posts. This avoids Reddit's RSS shutdown and does not rely on a third-party RSS converter.
- **Activity matters:** community choices were checked for recent posts. No active, dedicated Lemmy counterpart was found for Aseprite or homelab at the time of migration. Pixel Art covers general pixel-art work, including Aseprite-made art; the active self-hosting community also covers home servers and homelab projects. These are broader substitutes rather than exact one-to-one matches.
- Category names are intentionally unnumbered.

---

<div align="center">

*Collected and organised for a calmer, more useful reading workflow.*

</div>