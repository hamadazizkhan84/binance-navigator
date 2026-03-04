# 🟡 Binance Navigator AI — OpenClaw Skill

> Your personal crypto learning co-pilot. Built for the Binance × OpenClaw AI Competition (Mar 2026).

Binance Navigator is an OpenClaw skill that combines **live Binance market data** with an **AI-powered adaptive learning system**. It builds personalized crypto education roadmaps, tracks your Binance portfolio in real time, teaches concepts interactively, and quizzes you — all inside your OpenClaw assistant.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🗺 **Personalized Roadmap** | AI builds a custom 4-phase learning path based on your level and goals |
| 📊 **Live Market Data** | Real-time prices and 24hr stats direct from Binance API |
| 💼 **Portfolio View** | See your Binance balances and total portfolio value live |
| 📚 **Concept Teaching** | Interactive lessons across Crypto Basics, Binance Products, Trading & DeFi |
| 🧠 **Quiz Mode** | Multiple-choice quizzes with scoring and personalized feedback |
| 📈 **Trade History** | View your recent trades per symbol |
| 📉 **Candlestick Data** | Historical OHLCV data for any symbol and timeframe |
| ✅ **Progress Tracking** | Track completed topics and get next-step recommendations |

---

## 🚀 Installation

### Option 1 — Install via npx (recommended)
```bash
npx playbooks add skill openclaw/skills --skill binance-navigator
```

### Option 2 — Install via OpenClaw CLI
```bash
openclaw add @binance-navigator
```

### Option 3 — Manual install
```bash
# Clone into your OpenClaw skills folder
git clone https://github.com/YOUR_USERNAME/binance-navigator ~/.openclaw/workspace/skills/binance-navigator

# Then refresh skills in OpenClaw
openclaw agent --message "refresh skills"
```

---

## ⚙️ Setup

### 1. Get your Binance API Key
1. Log into [Binance.com](https://binance.com)
2. Go to **Profile → API Management**
3. Click **Create API**
4. Choose **System Generated**
5. Label it `openclaw-navigator`
6. Enable: ✅ Read Info only (no trading permissions needed for learning features)
7. Copy your **API Key** and **Secret Key**

### 2. Set environment variables
```bash
export BINANCE_API_KEY="your_api_key_here"
export BINANCE_SECRET="your_secret_here"
```

Or add to your OpenClaw config (`~/.openclaw/openclaw.json`):
```json
{
  "skills": {
    "entries": {
      "binance-navigator": {
        "enabled": true,
        "env": {
          "BINANCE_API_KEY": "your_api_key_here",
          "BINANCE_SECRET": "your_secret_here"
        }
      }
    }
  }
}
```

### 3. Requirements
- `curl` — pre-installed on macOS/Linux
- `jq` — install with `brew install jq` (macOS) or `apt install jq` (Linux)
- OpenClaw v2026 or later

---

## 💬 Usage Examples

Once installed, just talk to your OpenClaw assistant naturally:

```
You: start my learning path
Navigator: Let's build your roadmap! What's your experience level?...

You: what's the price of BTC?
Navigator: 🟡 BTC/USDT is currently $67,432.50 (+2.3% in 24h)

You: show my portfolio
Navigator: 💼 Your Binance Portfolio: BTC: 0.05 ($3,371) | ETH: 1.2 ($4,180)...

You: teach me about liquidity pools
Navigator: 📚 Liquidity Pools — think of it like a shared vending machine...

You: quiz me
Navigator: ❓ Question 1 of 3 — What does AMM stand for?...

You: how's the market today?
Navigator: 📊 Market Overview — BTC 🟢 +2.3% | ETH 🟢 +1.8% | BNB 🔴 -0.5%...
```

---

## 📁 File Structure

```
binance-navigator/
├── SKILL.md       ← OpenClaw skill definition (instructions + API tools)
├── README.md      ← This file
└── _meta.json     ← ClawHub registry metadata
```

---

## 🔐 Security

- This skill uses **read-only** Binance API access by default
- API keys are stored in your local OpenClaw environment only
- No data is sent to third parties — all API calls go directly to `api.binance.com`
- Never enable withdrawal permissions on the API key used with this skill

---

## ⚠️ Disclaimer

This skill is for **educational purposes only**. It does not provide financial advice. Crypto trading involves significant risk. Always do your own research before making investment decisions.

---

## 🏆 Competition Submission

Built for the **Binance × OpenClaw AI Competition** (Mar 4–18, 2026).

**Project:** Binance Navigator AI
**Category:** Crypto Educator / Binance UX Enhancement
**Focus:** All four tracks — Crypto Basics, Binance Products, Trading Strategy, DeFi & Web3

---

## 📄 License

MIT License — free to use, modify, and distribute.
