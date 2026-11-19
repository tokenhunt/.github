<h1 align="center">t◎kenhunt</h1>

<p align="center">
  <strong>Catch secrets at chat time, not commit time.</strong><br>
  Local-first secret scanning for AI coding agents. Fail-closed. Zero cloud, zero telemetry.
</p>

| project | what it is |
|---|---|
| **[token-hunt](https://github.com/tokenhunt/token-hunt)** | The engine — six hooks, 48 rules across 53 provider families, CLI (`scan / list / close / watch`), bash escape-hatch runtime detector |
| **[pat-scanner](https://github.com/tokenhunt/pat-scanner)** | The one-command Claude Code plugin — one hook, 13 credential classes, regex matching |
| **token-hunt-pro** | Silent redaction + active verification (GitHub / Stripe / Slack), offline ed25519 licensing — commercial |

```
pip install token-hunt
claude plugin install token-hunt@tokenhunt
```

<p align="center">
  <a href="https://tokenhunt.dev">tokenhunt.dev</a> ·
  <a href="https://tokenhunt.dev/docs">docs</a> ·
  <a href="https://tokenhunt.dev/changelog">changelog</a> ·
  <a href="https://x.com/tokenhuntdev">@tokenhuntdev</a> · info [at] tokenhunt.dev<br>
  <sub>BUSL-1.1 · MIT in 2030 · commercial by agreement</sub>
</p>
