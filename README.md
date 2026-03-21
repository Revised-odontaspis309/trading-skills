# Aelita Trader Skill

Live AI crypto trading signals for **Claude Code**, **OpenAI Codex**, and AI coding agents.

Powered by a production trading platform with multi-model MoE consensus, 15 real-time data dimensions, and automated signal verification.

**FREE during beta.**

## Install

### Claude Code

```bash
npx skills add roman-rr/aelita-trader-skill
```

### Manual

```bash
# Claude Code
cp SKILL.md ~/.claude/skills/aelita-trader/SKILL.md

# OpenAI Codex CLI
cp SKILL.md ~/.codex/skills/aelita-trader/SKILL.md
```

## What You Get

| Feature | Description |
|---------|-------------|
| Live signals | Bullish/bearish crypto signals with full trade setups |
| Entry / SL / TP | Exact price levels for every trade |
| Confidence score | 0-100 AI conviction level |
| Leverage | Suggested 1-10x leverage |
| Verification | Every signal tracked against real market prices |
| ROI tracking | Leverage-adjusted profit/loss per signal |
| Performance stats | Hit rate, cumulative ROI, breakdown by direction |

## Quick Start

```bash
# 1. Register (one-time)
curl -X POST https://aelita.x70.ai/api/skill/register \
  -H "Content-Type: application/json" \
  -d '{"name":"Your Name","email":"you@example.com","githubUrl":"https://github.com/you","purpose":"Portfolio tracker"}'

# 2. Get active signals
curl https://aelita.x70.ai/api/skill/signals?status=active \
  -H "X-Api-Key: ask_YOUR_KEY"

# 3. Check performance
curl https://aelita.x70.ai/api/skill/stats?days=30 \
  -H "X-Api-Key: ask_YOUR_KEY"
```

## API Endpoints

| Method | Path | Auth | Description |
|--------|------|------|-------------|
| POST | /api/skill/register | No | Register & get API key |
| GET | /api/skill/signals | API key | List signals (active/verified/all) |
| GET | /api/skill/signals/:id | API key | Single signal detail |
| GET | /api/skill/stats | API key | Performance statistics |

## Use Cases

- AI-powered portfolio rebalancing
- Trading bot signal feed
- Research and backtesting
- Market sentiment analysis
- Risk management dashboards

## Live Dashboard

Track real-time performance: https://aelita.x70.ai/signals/dashboard

## License

**Proprietary — Paid License Required for commercial redistribution.**

Free API access during beta. See [LICENSE.txt](./LICENSE.txt) for full terms.

## Author

**Roman Antonov**

- Email: romwtb@gmail.com
- GitHub: [github.com/roman-rr](https://github.com/roman-rr)
- Website: [roman-rr.github.io](https://roman-rr.github.io/)
