# 🟡 Binance Navigator AI
> A true crypto navigation co-pilot powered by OpenClaw — built for the Binance × OpenClaw AI Competition 2026

---

## What Is This?

Binance Navigator AI is an OpenClaw skill that acts as a **true navigator** to the Binance ecosystem. Instead of answering from AI memory, it fetches real data from official Binance sources and guides users directly to the right resources.

**Core Philosophy:** Every answer includes a real Binance link. The AI navigates — Binance educates.

---

## 8 Features

| Feature | Description | Data Source |
|---|---|---|
| 🗺 **Learning Journey Engine** | Assigns personalized week-by-week learning plans using real Binance Academy courses | Binance Academy |
| 📊 **Live Market Data** | Fetches real-time prices, 24hr stats, and market overview | Binance Public API |
| 📚 **Academy Navigator** | Finds the most relevant Binance Academy article for any topic | Binance Academy RSS |
| 🔗 **Product Navigator** | Links directly to exact Binance products with deep URLs | Binance.com |
| 📰 **News & Announcements** | Fetches latest from Binance blog and announcements | Binance Blog |
| 🧠 **Quiz Mode** | Quizzes users based on real Binance Academy content | Binance Academy |
| 🔍 **Glossary Lookup** | Instant definitions from Binance Academy glossary | Binance Academy |
| 🏆 **Learn & Earn Navigator** | Guides users to earn crypto rewards through Binance's program | Binance Learn & Earn |

---

## 4 Learning Journeys

Based on experience level and goals, users are assigned one of:

| Journey | For | Track | Duration | Certificate |
|---|---|---|---|---|
| 🌱 The Explorer | Beginners | Beginner Track | 4-6 weeks | NFT Certificate |
| 📈 The Trader | Some Experience | Intermediate Track | 6-8 weeks | NFT Certificate |
| 🌊 The DeFi Diver | Intermediate | Intermediate + BNB Chain | 8-10 weeks | Multiple |
| 🔨 The Builder | Advanced/Dev | BNB Developer Specialization | 12-16 weeks | Dev Certificate |

Each journey includes a week-by-week schedule with real module names, estimated times, and direct Academy links.

---

## Installation

### Requirements
- [OpenClaw](https://openclaw.ai) installed
- A Discord bot token
- A supported AI provider (Google Gemini recommended — free tier)

### Install

**Option 1 — Clone directly:**
```bash
cd ~/.openclaw/workspace/skills
git clone https://github.com/hamadazizkhan84/binance-navigator
```

**Option 2 — Manual:**
1. Download this repository
2. Copy the `binance-navigator` folder to `~/.openclaw/workspace/skills/`
3. Restart OpenClaw gateway: `openclaw gateway`

### Workspace Files
Also copy these to your `~/.openclaw/workspace/` directory:
- `AGENTS.md` — agent identity instructions
- `SOUL.md` — core behavior rules

---

## Usage Examples

```
@YourBot start                          → Full onboarding + journey assignment
@YourBot price of BTC                   → Live price from Binance API
@YourBot market overview                → Top 5 coins live data
@YourBot teach me about DeFi            → Real Binance Academy article
@YourBot what is APY?                   → Binance Academy glossary
@YourBot how do I start earning?        → Product navigator + direct link
@YourBot latest news                    → Binance blog + announcements
@YourBot quiz me                        → Quiz based on Academy content
@YourBot learn and earn                 → Learn & Earn portal guide
@YourBot next                           → Next module in their journey
```

---

## API Sources Used

All data comes from official Binance sources:

```
Live Prices:      https://api.binance.com/api/v3/ticker/24hr
Academy RSS:      https://api.binance.vision/api/feed
Academy Search:   https://academy.binance.com/en/search
Binance Blog:     https://www.binance.com/en/blog
Announcements:    https://www.binance.com/en/support/announcement
Learn & Earn:     https://www.binance.com/en/learn-and-earn
```

No private API keys required for core functionality.

---

## Competition Submission

Built for the **Binance × OpenClaw AI Competition (March 4-18, 2026)**

- 🔗 GitHub: https://github.com/hamadazizkhan84/binance-navigator
- 🐦 X Post: [link]
- 🎬 Demo Video: [link]

---

## Security

- No private Binance API keys required for core features
- All market data uses public Binance REST endpoints
- No user data is stored or transmitted
- Open source — fully auditable

---

## License

MIT License — free to use, modify, and distribute.

---

*Built with ❤️ for the Binance ecosystem*
