# Report Pipeline

Multi-client digital marketing reporting dashboard. Batch generates static HTML reports from analytics, advertising, and platform data.

## Architecture

```
connectors/
processors/
monitors/
ecosystem/
roadmap/
reporters/
db/
clients/
output/
```

## Data Sources

GA4, Google Search Console, Google Ads, ActiveCampaign, site crawler

## Report Types

Main analytics report, health monitor, ecosystem audit, prioritized roadmap

## Technology

Python, pandas, SQLite, Jinja2, Chart.js

## Flow

```
Client Config → Connectors → Processors → Reporters → HTML
                      ↕
                  SQLite DB
```

## Entry Points

| Script | Purpose |
|---|---|
| `run_client.py` | Unified runner — any report, any client |
| `main.py` | Legacy single-client runner |
| `run_health.py` | Standalone health report |
| `run_ecosystem.py` | Standalone ecosystem audit |
| `run_roadmap.py` | Standalone roadmap generator |
# ReportPipeline
Batch reporting pipeline that pulls and organizes digital marketing data.
