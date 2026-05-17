# Alpha Memo Forensics Engine

A local research-quality prototype for checking synthetic investment memo claims against evidence, freshness, contradiction, and traceability signals.

## Features

- Synthetic memo, catalyst, source, and market-signal records.
- Claim forensics for unsupported assertions, stale evidence, and contradiction risk.
- Verifiable reports, CSV findings, and an offline analytics dashboard.

## Run Locally

```bash
uv sync
uv run app init-demo
uv run app ingest fixtures/
uv run app analyze
uv run app verify
uv run app dashboard
uv run app benchmark
uv run app export-demo-pack
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/dashboard.html`
- `outputs/decision_report.md`
- `outputs/evidence_graph.mmd`
- `outputs/risk_or_quality_report.csv`
- `outputs/benchmark.md`
- `outputs/demo_pack.md`

## Data Policy

This project runs fully locally on deterministic synthetic fixtures. It does not require external APIs, credentials, private datasets, network access, or production systems.
