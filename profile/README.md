<div align="center">

# 🐾 KoshkiKode

**An indie studio building games, apps, and tools — one commit at a time.**

[![Website](https://img.shields.io/badge/Website-koshkikode.com-1a3c34?style=for-the-badge&logo=firefox&logoColor=white)](https://koshkikode.com)
[![Patreon](https://img.shields.io/badge/Patreon-Support_Us-FF424D?style=for-the-badge&logo=patreon)](https://patreon.com/koshkikode)
[![GitHub](https://img.shields.io/badge/GitHub-KoshkiKode-181717?style=for-the-badge&logo=github)](https://github.com/KoshkiKode)

</div>

---

## 👋 About KoshkiKode

KoshkiKode is an indie development studio crafting games, apps, and tools that are fun, functional, and built to last. We make things we'd want to use ourselves and share the whole journey along the way — design docs, devlogs, and all the messy bits in between.

Our projects range from games and marketplaces to local-first and educational tools. The studio website is a separate repository from the products.

| Project | What It Is |
|---------|------------|
| [**The Cordite Wars: Six Fronts**](#-the-cordite-wars-six-fronts) | Cross-platform real-time strategy game |
| [**Unshelv'd**](#-unshelvd) | Multilingual peer-to-peer book marketplace |
| [**Vetviona**](#-vetviona) | Local-first genealogy and research app |
| [**Untitled Trust Builder**](#-untitled-trust-builder) | Estate-planning information and document tools |
| [**PharmaSim**](#-pharmasim) | Educational drug-interaction and pharmacokinetic simulator |

The studio's static website is maintained separately in the [website repository](https://github.com/KoshkiKode/website).

---

## 🎮 The Cordite Wars: Six Fronts

> A cross-platform real-time strategy game inspired by Command & Conquer and Tempest Rising — currently in early development.

**Command across six simultaneous theatres of war.** Manage resources, deploy units, and outmanoeuvre your opponents across multiple fronts where every decision cascades. Deep tactical gameplay designed for replayability on PC, mobile, and everything in between.

### Key Features

- ⚔️ **Six Fronts** — six simultaneous theatres of war; losing one front shifts the balance on all others
- 🏗️ **Base Building** — construct and upgrade buildings, manage resource pipelines, and defend your perimeter
- 🤖 **Faction Asymmetry** — each faction has unique units, buildings, and playstyle
- 🌐 **Cross-Platform Multiplayer** — deterministic lockstep over LAN/local; identical simulation on every platform
- 📱 **Full Platform Coverage** — Windows, Linux, macOS, Android, iOS

### Tech Stack

| Layer | Technology |
|-------|-----------|
| Engine | Godot 4.6 with C# (.NET 9) |
| Simulation | Fixed-point math · deterministic xoshiro256\*\* RNG · 30 ticks/sec |
| Networking | LAN/local deterministic lockstep (no backend servers) |
| Platforms | Windows · Linux · macOS · Android · iOS |

### Links

[![Repo](https://img.shields.io/badge/Repo-cordite-181717?style=flat-square&logo=github)](https://github.com/KoshkiKode/cordite)

> 📣 Devlogs and playtest announcements will be posted on [Patreon](https://patreon.com/koshkikode).

---

## 📚 Unshelv'd

> **[unshelvd.koshkikode.com](https://unshelvd.koshkikode.com)**

**Where every book finds its next reader.**

Unshelv'd is a peer-to-peer book marketplace built for every language, every country, and every era. Buy, sell, trade, and discover books from fellow readers worldwide — with escrow-protected payments, 150+ languages, and a work-edition graph that automatically links every printing, translation, and edition of a book together.

### Key Features

- 🌍 **Global by Design** — 150+ languages, 30+ writing systems, 17 calendar systems, RTL support
- 🗺️ **Historical Nations** — Yugoslavia, USSR, Ottoman Empire, Austria-Hungary and more recognized as valid countries of origin
- 📖 **Work–Edition Graph** — every book automatically linked to all its editions, translations, and printings
- 🔍 **Book Requests** — post what you're looking for and get matched with sellers
- 💳 **Escrow Payments** — Stripe Connect + PayPal with buyer and seller protection
- 🖥️ **Web + Mobile** — React web app and Capacitor (Android/iOS); a desktop client is not implemented
- 🌐 **35 UI Languages** — top global languages with native labels

### Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React 19 · TypeScript · Tailwind CSS · shadcn/ui |
| Backend | Express.js · Passport.js · Stripe Connect · PayPal |
| Database | PostgreSQL · Drizzle ORM |
| Mobile | Capacitor (Android + iOS) |
| Desktop | Not implemented; Tauri setup is exploratory documentation |
| Hosting | Self-hosted · Debian · Docker Compose · Caddy · GoDaddy DNS |
| Catalog | Open Library API + proprietary database |

### Links

[![Website](https://img.shields.io/badge/Website-unshelvd.koshkikode.com-1a3c34?style=flat-square&logo=firefox&logoColor=white)](https://unshelvd.koshkikode.com)
[![Repo](https://img.shields.io/badge/Repo-unshelvd-181717?style=flat-square&logo=github)](https://github.com/KoshkiKode/unshelvd)

> Check the product site for current availability and terms.

---

## 🌿 Vetviona

> **[vetviona.koshkikode.com](https://vetviona.koshkikode.com)**

**Your family history, beautifully organized.**

Vetviona is a private, local-first genealogy app. Build interactive family trees, attach source citations, and sync across all your devices — completely without a server you need to maintain. Available on every major platform with a simple one-time purchase.

### Key Features

- 🌳 **Interactive Tree Builder** — add people, link parents/children and spouses, pan & zoom
- 📚 **Source Citations** — attach evidence to birth, marriage, and death facts
- 📍 **Historical Place Matching** — date-aware autocomplete that understands changing borders and names over time
- 🔄 **RootLoop™ Sync** — encrypted device-to-device sync (no external server)
  - **RootLoop™ Auto** — full WiFi sync that runs automatically on your home network
  - **RootLoop™ Manual** — on-demand Bluetooth/local sync you trigger yourself
- 📤 **GEDCOM Import & Export** — industry-standard format; import your existing tree from any app
- 📄 **PDF Family Book** — generate a narrative-style PDF of your whole tree
- ⏱️ **Life Timelines** — view an individual's key life events chronologically
- 🔍 **Relationship Finder** — instantly see how any two people in your tree are related
- 🔒 **Local PIN Protection** — optional username/password lock for on-device privacy

The project describes one-time purchase options. See the product site for current pricing and platform availability.

### Tech Stack

| Layer | Technology |
|-------|-----------|
| App | Flutter (Dart) · multi-platform |
| Sync | RootLoop™ v1.0.0 — WiFi + Bluetooth, zero-knowledge encrypted |
| Backend | Node.js license/account service verifies downloaded paid builds and desktop; app-store purchases use store receipts. Local editing and device-to-device sync do not depend on the service. |
| Packaging | WiX (Windows) · Notarized DMG (macOS) · DEB + Snap + Flatpak (Linux) |

### Links

[![Website](https://img.shields.io/badge/Website-vetviona.koshkikode.com-1a3c34?style=flat-square&logo=firefox&logoColor=white)](https://vetviona.koshkikode.com)
[![Repo](https://img.shields.io/badge/Repo-vetviona-181717?style=flat-square&logo=github)](https://github.com/KoshkiKode/vetviona)

---

## 🏡 Untitled Trust Builder

> An estate-planning information and document-template app.

Untitled Trust Builder guides users through questions about trusts, LLCs, and property to produce state-aware planning information, cost and risk estimates, and downloadable PDFs. It is **not legal advice**; generated materials are informational and should be reviewed with a qualified professional. The app is designed to keep user data on the device.

### Links

[![Repo](https://img.shields.io/badge/Repo-untitled--trust--builder-181717?style=flat-square&logo=github)](https://github.com/KoshkiKode/untitled-trust-builder)

---

## 💊 PharmaSim

> An educational, client-side drug-interaction and pharmacokinetic simulator.

PharmaSim includes a library of more than 880 substances, patient profiles, pharmacokinetic timelines and curves, and rule-based interaction and toxicity outputs. It is **not for medical use** and must not be used to guide treatment. Use only fictional, non-identifying data; the project describes local-only storage and no account or cloud sync.

### Links

[![Repo](https://img.shields.io/badge/Repo-pharmasim-181717?style=flat-square&logo=github)](https://github.com/KoshkiKode/pharmasim)

---

## 🤝 Support the Studio

KoshkiKode is a small independent studio. If you enjoy what we're building, supporting us on Patreon directly funds development time, tooling, and keeps the projects alive.

<div align="center">

[![Become a Patron](https://img.shields.io/badge/Become_a_Patron-FF424D?style=for-the-badge&logo=patreon&logoColor=white)](https://patreon.com/koshkikode)

</div>

---

## 📬 Connect

| Platform | Link |
|----------|------|
| 🌐 Website | [koshkikode.com](https://koshkikode.com) |
| 🎮 Patreon | [patreon.com/koshkikode](https://patreon.com/koshkikode) |
| 🏡 Trust Builder | [Repository](https://github.com/KoshkiKode/untitled-trust-builder) |
| 💊 PharmaSim | [Repository](https://github.com/KoshkiKode/pharmasim) |
| 📖 Unshelv'd | [unshelvd.koshkikode.com](https://unshelvd.koshkikode.com) |
| 🌿 Vetviona | [vetviona.koshkikode.com](https://vetviona.koshkikode.com) |
| 🐙 GitHub | [github.com/KoshkiKode](https://github.com/KoshkiKode) |

---

<div align="center">

*Made with ☕ and too many late nights by KoshkiKode*

</div>
