<h1 align="center">Readia SDK</h1>

<p align="center">
  <strong>Content commerce infrastructure for humans and AI agents.</strong>
</p>

<p align="center">
  <a href="https://readia.io/sdk">Documentation</a> •
  <a href="https://readia.io/docs">API Reference</a> •
  <a href="https://readia.io">Website</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-coming%20soon-yellow" alt="Status: Coming Soon" />
  <img src="https://img.shields.io/badge/license-MIT-blue" alt="License: MIT" />
</p>

---

## 🚧 Coming Soon

The Readia SDK is currently in development. Star this repo to be notified when we launch.

---

## What is Readia SDK?

The Readia SDK enables developers to integrate **x402-powered content commerce** into any application. Build platforms where creators get paid instantly — whether the consumer is a human or an AI agent.

### Key Features

- **x402 Protocol** — Native support for machine-readable payments
- **Multi-Chain** — USDC on Base and Solana, plus custom token support
- **Instant Settlement** — Payments flow directly from consumer to creator
- **Agent-Ready** — Built for both human users and AI agents
- **TypeScript First** — Full type safety and modern DX

---

## Quick Preview

```typescript
import { Readia } from '@readia/sdk'

// Initialize the SDK
const readia = new Readia({
  network: 'base',
  apiKey: process.env.READIA_API_KEY
})

// Publish monetized content
const article = await readia.publish({
  title: 'Getting Started with Web3',
  content: markdownContent,
  price: 0.10  // $0.10 USDC
})

// Handle x402 payments automatically
app.get('/article/:id', readia.paywall(), (req, res) => {
  // Only reached after payment verification
  res.json({ content: article.content })
})
```

---

## Use Cases

| Use Case | Description |
|----------|-------------|
| **Content Platforms** | Monetize articles, tutorials, research with per-piece pricing |
| **AI Agent Infrastructure** | Enable agents to pay for and publish content programmatically |
| **Creator Tools** | Build publishing tools with built-in monetization |
| **Data Marketplaces** | Sell datasets, APIs, or digital assets with instant settlement |

---

## Networks Supported

| Network | Tokens |
|---------|--------|
| Base | USDC |
| Solana | USDC, $READ |

---

## Get Notified

⭐ **Star this repo** to be notified when we launch.

📬 **Join the community:**
- [Twitter/X](https://twitter.com/readia_io)
- [Telegram](https://t.me/readia_official)

---

## Links

- [Readia Website](https://readia.io)
- [SDK Overview](https://readia.io/sdk)
- [$READ Token](https://readia.io/token)
- [Roadmap](https://readia.io/roadmap)

---

<p align="center">
  <sub>Built by <a href="https://readia.io">Readia LLC</a></sub>
</p>
