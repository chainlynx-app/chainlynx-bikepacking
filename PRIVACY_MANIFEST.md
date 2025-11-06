# ChainLynx Privacy Manifest  
### *Private by default. Shared only by choice.*

ChainLynx Bikepacking is designed around privacy, user ownership, and transparency.  
It follows a hybrid, privacy-first architecture that ensures your data remains under your control — not ours.

---

## Overview

ChainLynx lets riders connect, share, and explore — while keeping personal information secure.  
Your data never powers ads, recommendations, or tracking systems.  
You decide what gets shared, who sees it, and when.

---

## Data Architecture

ChainLynx uses a **hybrid, privacy-first model** combining local storage, personal cloud, and minimal shared backend services.

| Layer | Description |
|--------|-------------|
| **Device** | Stores all personal data locally — routes, journals, preferences, AI interactions, and cached map data. |
| **Personal Cloud (User-Owned)** | Optional sync for journals and backups to your own iCloud, Google Drive, or OneDrive account. |
| **Community Cloud (Shared Data)** | Hosts anonymized community content such as trail reports, meetups, POIs, and shared journals. No personal identifiers are stored. |
| **Object Storage** | Stores shared photos and videos using direct upload links (pre-signed URLs). Files never pass through ChainLynx’s backend. |
| **Ephemeral GPS Layer** | Handles live location sharing during active sessions; data is temporary and deleted automatically after sharing stops. |

---

## Journals

- **Private by default:** Your journals live only on your device or your chosen cloud storage.  
- **Optional sharing:** You may share specific journal entries with selected users or the public feed. Only that shared content is uploaded — not your entire journal.  
- **Encryption:** All journals and backups are encrypted locally before upload.  
- **Control:** You can revoke shared access or delete shared journals at any time.

---

## Location Sharing

- **Opt-in only:** Location sharing is entirely voluntary.  
- **Visibility options:**
  - *Meetup group:* Share with a specific group of riders.  
  - *Route peers:* Share with all users currently on the same route.  
- **Data source:** Uses device GPS or connected Garmin inReach MapShare feed.  
- **Ephemeral data:** Positions are transmitted securely via TLS and automatically deleted after each session.  
- **No tracking:** ChainLynx does not log or reconstruct travel history.

---

## Messaging

- **End-to-End Encryption (E2EE):** Messages are encrypted using the Signal Protocol.  
- **Relay-only backend:** Servers can relay encrypted messages but cannot read or store them.  
- **Temporary delivery:** Messages are deleted from the relay once delivered to the recipient.  
- **Backup security:** Optional encrypted backups to your own cloud storage using a user-held recovery key.

---

## Offline AI Assistants

- **On-device processing:** All AI assistants (e.g., *AI Bike Mechanic*, *Campmaster*) run locally using TensorFlow Lite or ONNX Runtime.  
- **No data transmission:** Prompts and responses are processed entirely on the device.  
- **Optional model downloads:** Users can install or remove small specialized models for offline use.  
- **Transparency:** No AI queries or analytics are sent to external servers.

---

## Personal Cloud Storage

Each user owns their storage space.  
At launch, ChainLynx supports:
- iCloud (Apple)
- Google Drive
- OneDrive

The storage system is modular and will expand to support additional privacy-friendly options such as Nextcloud, Dropbox, and WebDAV in future versions.

---

## Encryption and Security

| Data Type | Encryption | Storage | Notes |
|------------|-------------|----------|-------|
| **Messages** | Signal Protocol (E2EE) | Sender/Recipient devices | Relay cannot decrypt messages. |
| **Journals & Backups** | AES-256 | Local / User cloud | Encrypted before upload. |
| **Trail Reports & Posts** | TLS 1.3 | Community backend | Stored anonymously with hashed IDs. |
| **Photos/Videos** | TLS 1.3 | Object storage | Uploaded via pre-signed URLs. |
| **AI Models** | Local encryption | Device | No online processing. |
| **Location Data** | TLS 1.3 (in transit) | Ephemeral GPS cache | Deleted automatically after session ends. |

---

## Data Ownership Summary

| Data Type | Default State | Who Owns It | Who Can Access | Retention |
|------------|----------------|-------------|----------------|------------|
| **Journals** | Private | User | User | Persistent (user-controlled) |
| **Shared Journals** | Opt-in | User | Selected users / public | Until revoked |
| **Trail Reports** | Public | User | Public | Persistent, anonymized |
| **Messages** | Private | Users | Sender + Recipient | Temporary |
| **Meetup Info** | Limited-share | User | Group members | Session-based |
| **Live Location** | Opt-in | User | Group or route peers | Temporary |
| **AI Interactions** | Private | User | User | Local only |

---

## Core Privacy Principles

1. **Private by Default** — nothing is shared without user action.  
2. **Shared by Choice** — every sharing action is explicit and reversible.  
3. **Anonymized by Design** — all community data uses hashed, non-identifiable IDs.  
4. **User-Owned Storage** — personal data lives in your own cloud, never ours.  
5. **End-to-End Encryption** — messages and backups are always encrypted before leaving your device.  
6. **No Tracking, No Ads, No Analytics** — ChainLynx collects no telemetry or behavioral data.  
7. **Open Documentation** — privacy design and architecture are fully public.

---

## Technical Safeguards

- AES-256 encryption for all local and backup data.  
- TLS 1.3 for secure data transmission.  
- OAuth authentication with hashed IDs (no passwords stored).  
- Pre-signed upload URLs for file isolation.  
- Automatic deletion of ephemeral GPS data.  
- Strict data segmentation between private and shared layers.  
- Open, auditable architecture.

---

## Transparency & Auditing

ChainLynx’s privacy model, architecture, and encryption strategies are open-source and publicly documented.  
Community members are encouraged to review, test, and contribute to privacy improvements.  

A **Privacy Review Board** will periodically publish independent audits and community-led reviews of data handling practices.

---

## Version

**Privacy Manifest v1.1** — November 2025  
Aligned with:  
- *Architecture Overview: A Hybrid, Privacy-First Model*  
- *Messaging.pdf*  
- *Technical Implementation Options for Offline AI.pdf*  

---

> *ChainLynx Bikepacking — The social network for the wild. Private by default. Shared only by choice.*
