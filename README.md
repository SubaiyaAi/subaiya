# Subaiya

**The universal security layer for AI agents.**

Subaiya is designed to work with any AI client. The most dangerous actions can't exist. Everything else, you control.

## What it does

- **Prompt Injection Shield:** Detects hidden instructions in files, emails, and websites before your agent can process them
- **20 Permission Categories:** Files, terminal, email, browser, payments, and 15 more. Each configurable with On, Ask, or Off
- **Identity Guard:** Agent personality files (SOUL.md, IDENTITY.md) are read-only and tamper-proof
- **Live Dashboard:** Real-time activity feed. See every action your agent takes
- **Session Budget Control:** Prevent runaway API costs
- **Emergency Stop:** One click to stop your agent
- **4 Presets:** Strict, Normal, Relaxed, Custom

## Supported Models

| Model | Status |
|-------|--------|
| Anthropic | ✅ Supported |
| OpenAI | ✅ Supported |
| Gemini, DeepSeek, and more | 🟡 Planned |

## Integrations

| AI Client | Status |
|-----------|--------|
| OpenClaw | ✅ Live |
| More clients | 🟡 Planned |

## Quick Start

1. **Register** at [subaiya.com](https://subaiya.com) (free during beta)
2. **Add Subaiya** as a provider in your OpenClaw config:
   ```json
   {
     "providers": [{
       "name": "subaiya",
       "baseUrl": "https://api.subaiya.com/t/YOUR-KEY",
       "models": [{"id": "claude-sonnet-4-6"}]
     }]
   }
   ```
3. **Open your dashboard** and set your rules

Full setup guide: [subaiya.com/docs](https://subaiya.com/docs)

## Architecture

Subaiya is a proxy. No code is installed on your machine. Your API key is encrypted at rest and passed through to your AI provider. We never store conversations, prompts, or responses.

## Privacy

- EU servers (Hetzner, Germany)
- GDPR compliant
- No tracking, no cookies (except auth session)
- Passwords hashed with Argon2id
- API keys encrypted with Fernet/AES-128-CBC

## Links

- **Website:** [subaiya.com](https://subaiya.com)
- **Documentation:** [subaiya.com/docs](https://subaiya.com/docs)
- **Dashboard:** [subaiya.com/dashboard](https://subaiya.com/dashboard)
- **Contact:** info@subaiya.com

## Status

Subaiya is in beta. Currently live with OpenClaw as the first integration. More AI clients coming soon.

## License

Subaiya is a proprietary service. This repository is for documentation, issue tracking, and community discussion.
