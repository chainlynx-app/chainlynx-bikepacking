# ChainLynx: The Bikepacking Companion
**The offline, privacy-first social network for bikepackers.**  
Built for the wild, not the algorithm.�

---

## About

**ChainLynx** connects riders through routes, journals, meetups, and trail reports — all built around privacy and offline-first technology.  
It’s part mapping tool, part journal, part social network — designed to work anywhere, even without a signal.

At its core, ChainLynx is guided by one principle:  
> Private by default. Shared only by choice.

---

>  *ChainLynx isn’t just another app — it’s a movement toward ethical, open, and human-centered technology for the outdoors.*

---

##  Project Goals

1. **Build a privacy-respecting social layer for outdoor explorers**  
   ChainLynx aims to become a trusted space for bikepackers and bicycle tourers to connect — without sacrificing their privacy.  
   Every interaction, from sharing a journal to posting a trail update, is governed by user choice and data transparency.  
   No algorithms, trackers, or advertising networks. Just people sharing genuine experiences.

2. **Demonstrate that offline-first, community-driven tech can be beautiful and functional**  
   Modern apps don’t have to rely on constant connectivity or surveillance capitalism to deliver great user experiences.  
   ChainLynx is designed to perform seamlessly offline — offering maps, AI tools, messaging, and data sync even in remote areas.  
   It’s proof that ethical design and cutting-edge technology can coexist.

3. **Develop a sustainable open platform powered by its users — not ads or data harvesting**  
   The long-term vision is for ChainLynx to grow as a decentralized, open-source ecosystem.  
   Contributors, not corporations, shape its roadmap.  
   The platform is free to use, community-funded, and transparent about every line of code and every server it runs.

4. **Empower real-world connection and safety through responsible technology**  
   ChainLynx isn’t just about digital sharing — it’s about enabling meaningful encounters outdoors.  
   Features like meetups, live location sharing, and encrypted messaging foster genuine community and real-time safety support on the trail.

5. **Champion data sovereignty and interoperability**  
   All personal content — routes, journals, and backups — remains under the user’s control.  
   The app integrates with user-owned cloud storage (iCloud, Google Drive, OneDrive) and will expand to privacy-friendly providers like Nextcloud or WebDAV.  
   Data is stored in open, portable formats (GPX, Markdown, JSON), ensuring users are never locked in.

6. **Advance open, ethical innovation in outdoor and mapping technology**  
   By developing open standards for offline mapping, encrypted messaging, and edge AI, ChainLynx aims to inspire a new wave of responsible outdoor technology.  
   The project will serve as a model for how open-source communities can collaborate on privacy-first software that directly benefits its users.

7. **Foster a global, inclusive outdoor community**  
   ChainLynx encourages knowledge exchange between riders from different regions and backgrounds.  
   It’s designed to scale globally while respecting local contexts — supporting multilingual content, regional route libraries, and culturally aware communication.


---

## Features Overview

| Category | Description |
|-----------|-------------|
| **Offline Routes** | Download full map tiles, GPX tracks, elevation data, POIs and route description for offline use. |
| **Journals** | Keep personal ride logs locally or in your own cloud. You can choose to keep journals private or share them publicly or with specific riders. |
| **Meetups & Live Location** | Share your GPS position (or Garmin inReach MapShare) with your meetup group or everyone on a route. Location sharing is optional and temporary. |
| **Trail Reports Feed** | Post or view real-time reports — conditions, hazards, or tips — shared anonymously. |
| **Community Feed** | A simple, chronological feed where riders can share posts, photos, and updates from their trips. No algorithms, no ads — just real stories from the trail. |
| **Private Messaging** | End-to-End Encrypted using the Signal Protocol. The server only relays encrypted messages. |
| **Offline AI Assistants** | Optional on-device AI packs like *AI Bike Mechanic*, *Wildreness Medic* or *Campmaster* for offline help. |

---

## Privacy-First Architecture

ChainLynx is built on a **hybrid, privacy-first model** designed to give every user full control over their own data — while still enabling community interaction and collaboration.

### Core Principles
- **Private by default:** All journals, preferences, and messages are stored locally and encrypted. Nothing is shared unless the user explicitly chooses to.  
- **Shared by choice:** When a user shares a journal, location, or trail report, only that specific content is uploaded — not their full account or metadata.  
- **Minimal backend:** The central server stores only community-level data (trail reports, meetups, POIs, shared journals). It contains no personal identifiers.  
- **Ephemeral location:** Live GPS updates and inReach MapShare feeds are visible only to users who have opted in and are erased once a session ends.  
- **On-device intelligence:** All AI assistants (e.g., *AI Bike Mechanic*, *Campmaster*) run locally on the user’s device — no prompts or responses are sent to any cloud service.

### Personal Cloud Storage
Every user owns their personal data store.  
ChainLynx connects directly to the user’s preferred cloud provider and saves data into a secure, app-specific folder.  
At launch, supported providers are:
- **iCloud** (Apple)
- **Google Drive**
- **OneDrive**

The storage layer is modular — future releases will allow additional adapters for **Nextcloud**, **Dropbox**, **WebDAV**, or even self-hosted storage options.  
This design ensures that users always know where their data lives and who can access it.

### Encryption & Anonymity
- **Messages:** Encrypted end-to-end using the Signal Protocol; the server only relays ciphertext.  
- **Cloud Backups:** Encrypted locally before upload with AES-256.  
- **Community Posts:** Stored with hashed, anonymous IDs — never linked to emails or real names.  
- **Data in Transit:** Protected with TLS 1.3.  

### Hybrid Data Flow
| Layer | Description |
|--------|-------------|
| **Device** | Stores all private data locally; handles offline maps, AI, and encryption. |
| **Personal Cloud** | Optional sync for journals and backups — user-owned storage only. |
| **Community Cloud** | Hosts shared POIs, reports, meetups, and anonymized posts. |
| **Object Storage** | Stores shared photos/videos directly via pre-signed URLs. |
| **Ephemeral GPS Layer** | Handles live location sharing; clears automatically after session ends. |

### Transparency Promise
ChainLynx is architecturally incapable of reading personal journals, messages, or backups.  
All sharing actions are explicit and reversible.  
A detailed data-handling explanation is available in the [Privacy Manifest](./PRIVACY_MANIFEST.md).

---

## Current Status

**Pre-Release Phase**

The project is shared publicly for transparency and collaboration.  
At this stage:
- Forking and redistribution are disabled.  
- Commercial use is **not permitted**.  
- Collaboration via pull requests and discussions is welcome.

When the first stable release is ready, ChainLynx will transition to a full open-source license (MIT or AGPL).

---

## Contributing

You can help shape ChainLynx:
1. Join the conversation in **Discussions** or **Issues**.  
2. Share design, UX, and feature feedback.  
3. Test prototypes and give real-world insights.

---

## Documentation

- [Privacy Manifest](./PRIVACY_MANIFEST.md)  
- [Architecture Overview](./docs/Architecture%20Overview.pdf)  
- [Offline AI Implementation Options](./docs/Technical%20Implementation%20Options%20for%20Offline%20AI.pdf)  
- [Colour Palette & Branding](./branding/Colour%20Palette.pdf)

---

## Roadmap

| Phase | Focus | Status |
|--------|--------|--------|
| 1 | Core React Native scaffolding | 🟢 In progress |
| 2 | Offline route and map system | ⚪ Planned |
| 3 | Feed, Meetups, Journal sharing | ⚪ Planned |
| 4 | Secure messaging (Signal E2EE) | ⚪ Planned |
| 5 | Offline AI assistants | ⚪ Planned |
| 6 | Beta release | ⚪ Future |

---

## Legal Notice

This project is currently in its **pre-release** stage.  
**All rights are reserved** by the ChainLynx maintainers.

You may:
- View the repository  
- Submit issues or pull requests  
- Participate in design and feedback

You may **not**:
- Redistribute, fork, or modify this repository  
- Use any part of this project for commercial purposes

A full open-source license will be added when the stable version is released.  
For questions or permissions, contact **chainlynx.app@gmail.com**.

---

## Connect

- Website: *coming soon*  
- Email: **chainlynx.app@gmail.com**  
- Socials: *coming soon*

> *ChainLynx — The social network for the wild.*
