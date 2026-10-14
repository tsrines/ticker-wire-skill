# ticker-wire-skill

Grok Bot / agent skill for **Ticker Wire** - stocks-only company news alerts
via a hosted watcher that emails the bot's Grok Bot inbox (webhook optional).

## Install

```bash
npx skills add tsrines/ticker-wire-skill -g
```

Or with an explicit skill name:

```bash
npx skills add tsrines/ticker-wire-skill --skill ticker-wire -g -y
```

Lands at `~/.agents/skills/ticker-wire` (global).

## Package layout

```
skills/ticker-wire/SKILL.md          # primary: getting started + operator section
skills/ticker-wire/references/getting-started.md
skills/ticker-wire/references/feed-setup.md
skills/ticker-wire/references/watchlist.md
```

## Scope

- Stocks only (no crypto until shipped)
- Hosted watcher via `WATCHER_BASE_URL`
- Email-first delivery to the bot's own Grok Bot inbox; webhook optional (sender key via secret-request only)
- Watchlist chat ops (add/remove/list/what's-new); desk-line alerts on hits
- No Zapier / third-party automation tours
- No PII in skill prose
