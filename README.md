# ChainLynx: The Traveling Cyclist’s Companion  
**The offline, privacy-first social network for bikepackers and touring cyclists.**  
Built for the wild, not the algorithm.  

---

> **Prototype Notice**  
> The app and explainer video showcase a **functional mockup** demonstrating how ChainLynx will look and feel.  
> The current codebase focuses on core architecture, offline scaffolding, and contributor setup.  
> We’re inviting developers, designers, and riders to help make it real.  

---

## About  

**ChainLynx** connects cyclists through routes, journals, meetups, and trail reports — all built around **privacy** and **offline-first** design.  
It’s part navigation tool, part journal, part community — built to work anywhere, even without a signal.  

At its core, ChainLynx follows one simple principle:  
> **Private by default. Shared only by choice.**

---

> *ChainLynx isn’t just another cycling app — it’s a movement toward ethical, open, and human-centered technology for the outdoors.*  

---

## Vision & Goals  

1. **Build a privacy-respecting social layer for outdoor explorers**  
   A trusted, ad-free space for bikepackers and touring cyclists to connect. Every post, report, or journal entry is shared only by user choice — never tracked, sold, or algorithm-curated.  

2. **Demonstrate that offline-first, community-driven tech can be beautiful and functional**  
   ChainLynx works seamlessly without connectivity, offering offline maps, AI tools, and journals synced safely when a connection returns.  

3. **Develop a sustainable open platform powered by its users — not ads or data harvesting**  
   The project is open-source and community-driven. Contributors, not corporations, shape the roadmap.  

4. **Empower real-world connection and safety through responsible technology**  
   Features like meetups, live location sharing, and encrypted messaging enable genuine community and safety support on the road.  

5. **Champion data sovereignty and interoperability**  
   Users own their data through personal cloud storage — iCloud, Google Drive, or OneDrive — with future support for Nextcloud, WebDAV, and self-hosting.  

6. **Advance open, ethical innovation in mapping and outdoor technology**  
   ChainLynx pioneers offline AI tools, encrypted communication, and open standards for a fairer outdoor tech ecosystem.  

7. **Foster a global, inclusive cycling community**  
   Designed for cultural and geographic diversity, ChainLynx connects cyclists worldwide while respecting local context and accessibility.  

---

## Features Overview  

| Category | Description |
|-----------|-------------|
| **Journey Mode** | Record and share flexible, open-ended tours. ChainLynx can track your path, letting you add notes, reports and journals, and connect with nearby riders — ideal for bicycle nomads and tourers. |
| **Offline Routes** | Explore curated bikepacking routes with full offline map tiles, GPX data, POIs, and elevation profiles. |
| **Journals** | Keep personal ride logs locally or in your cloud. Choose to keep them private or share selected entries. |
| **Meetups & Live Location** | Share your GPS position (or Garmin inReach MapShare) with your group or other riders nearby. Fully opt-in and temporary. |
| **Trail Reports Feed** | Post or view real-time reports — conditions, hazards, or detours — shared anonymously for community safety. |
| **Private Messaging** | End-to-End Encrypted using the Signal Protocol. The server never stores readable messages. |
| **Offline AI Assistants** | On-device helpers such as *AI Bike Mechanic*, *Wilderness Medic*, and *Campmaster* — all functional offline and privacy-safe. |

---

## Privacy-First Architecture  

ChainLynx is built on a **hybrid, privacy-first model**, giving every user full control of their data while still enabling community connection.  

### Core Principles  
- **Private by default:** All journals, preferences, and messages remain encrypted on-device.  
- **Shared by choice:** Only explicitly shared content — a post, location, or report — is uploaded.  
- **Minimal backend:** The central server only handles public data (reports, meetups, POIs). No personal identifiers.  
- **Ephemeral location:** Shared GPS data auto-expires after the session ends.  
- **On-device intelligence:** All AI assistants operate locally; no queries leave the device.  

### Personal Cloud Storage  
Users connect their preferred cloud service:  
- iCloud (Apple)  
- Google Drive  
- OneDrive  

Upcoming support: Nextcloud, Dropbox, WebDAV, and self-hosted sync.  
This ensures users always know *where* their data lives and *who* can access it.  

### Security Highlights  
- **E2E Messaging:** Signal Protocol encryption.  
- **Local Cloud Encryption:** AES-256 before upload.  
- **Anonymized Community Posts:** Hash-based user IDs.  
- **Secure Transmission:** TLS 1.3 for all connections.  

---

## Current Status  

**Phase 1 — Active Development**  

The project is in its pre-release phase and actively seeking contributors.  
You can explore the codebase, follow technical documentation, and contribute through Issues or Pull Requests.  

- ChainLynx will remain **free and open-source forever.**  
- **Commercial use, monetization, or resale are permanently prohibited.**  
- Contributions follow the repository’s `CONTRIBUTING.md`.  

---

## Contributing  

You can help shape ChainLynx:  
1. Join the discussion in **Issues** or **Discussions**.  
2. Suggest UX, feature, or privacy improvements.  
3. Contribute code — frontend (React Native), backend (Node.js + PostGIS), or AI integration.  

### Developer Quick Start  
| Tool | Purpose |
|------|----------|
| **Expo CLI** | Launch and test mobile builds |
| **Docker Compose** | Run backend and database locally |
| **Node.js + PostgreSQL/PostGIS** | API and spatial data store |
| **VS Code / GitHub Actions** | Development and CI/CD tools |

Full setup instructions are in [`CONTRIBUTING.md`](./CONTRIBUTING.md).  

---

## Roadmap  

| Phase | Focus | Timeframe | Status |
|-------|--------|------------|--------|
| 1 | Core Foundation — scaffolding, offline maps, authentication | Months 0–3 | 🟢 In progress |
| 2 | Essential Features — journals, feed, trail reports, offline AI prototypes | Months 3–6 | ⚪ Planned |
| 3 | Community & Sharing — meetups, route uploads, shared journals | Months 6–9 | ⚪ Planned |
| 4 | Integrations & Optimization — Garmin/Wahoo, performance, privacy audit | Months 9–12 | ⚪ Planned |

See the full technical [Development Roadmap](./docs/Development_Roadmap.pdf) for detailed milestones and contributor roles.  

---

## Licensing & Usage Policy  

ChainLynx is a **non-commercial, community-driven project**.  
It will remain **free and open-source forever** under a custom license that:  

- **Prohibits all commercial use** (no resale, monetization, or paid derivatives).  
- **Encourages educational, research, and community contributions.**  
- **Protects user privacy and data sovereignty as a core principle.**  

Any derivative or fork must also remain non-commercial and uphold the same privacy-first ethos.  

---

## Connect  

- Website: *coming soon*  
- Email: **chainlynx.app@gmail.com**  
- Socials: *coming soon*  
- Full documentation: [docs/README.md](./docs/README.md)  
- Executive Summary: [Executive_Summary.pdf](./docs/Executive_Summary.pdf)  

---

> *ChainLynx — The social network for the wild.*  
