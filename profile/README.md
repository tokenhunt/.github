# tokenhunt

**Catch secrets at chat time, not commit time.**

Secret scanning for AI coding agents. Six hooks, fail-closed, zero cloud,
zero telemetry. The transcript is the leak surface.

| | |
|---|---|
| Docs | <https://tokenhunt.dev/docs> |
| Changelog | <https://tokenhunt.dev/changelog> |
| License | BUSL-1.1 · MIT in 2030 · commercial by agreement |

## The products

**Engine**

- [`token-hunt`](https://github.com/tokenhunt/token-hunt) — the CLI
  (`scan / list / close / watch`), six hooks with block-and-rotate behavior,
  the allowlist, and the bash escape-hatch runtime detector no regex can see

**Plugins**

- [`pat-scanner`](https://github.com/tokenhunt/pat-scanner) — the
  one-command Claude Code plugin: one hook, 13 credential classes, regex
  matching. The guard, without the workflow.

**Commercial**

- `token-hunt-pro` — silent redaction (the agent never sees the raw value)
  + active verification against GitHub / Stripe / Slack, offline ed25519
  licensing. Zero phone-home.

## The checkable claims

- 48 credential rules across 53 provider families, local-only
- BLOCK hooks stop the tool call before it runs, not after it logs
- the escape-hatch class (`${VAR:+SET}${VAR:-UNSET}`) is caught by the
  runtime detector — regex can't see it
- everything runs on your machine — zero telemetry
```
pip install token-hunt
claude plugin install token-hunt@tokenhunt
```
