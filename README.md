<div align="center">

# Sajad Roudbari

### Forward Deployed Engineer / Solutions Architect

Tehran, Iran &nbsp;·&nbsp; Open to relocation

[![Website](https://img.shields.io/badge/iamsajaad.com-24292F?style=flat-square&logo=safari&logoColor=white)](https://iamsajaad.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/iamsajaad)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:sajad.rudbari@gmail.com)

</div>

---

> I go into messy environments, get access, ship working systems end to end, and then run them in production.

Analytics platforms, LLM pipelines, payment integrations. Most of what I have shipped started as a problem nobody owned, with no mandate to fix it.

<br>

## Production systems I own

#### Zonerift &nbsp;·&nbsp; built and operated solo

A privacy service that picks the exit region per service rather than routing everything through one IP, and switches mid-session without dropping the connection. WireGuard across **18 AWS regions** provisioned with Ansible, PostgreSQL and Redis behind a Python REST API, payments across 10+ fiat and crypto rails with no third-party billing provider.

**~1.5 PB/month at 99.9% uptime, effectively unattended.** AWS funded the first year of infrastructure.

#### Call intelligence at Digikala &nbsp;·&nbsp; Quick Commerce

Quality control ran on a random 10% sample of call-centre calls, and escalation was how anything outside that sample got found. I negotiated archive access out of the company's most regulation-bound data team, then built a pipeline over the **full daily volume**: transcription, sentiment, and three compliance categories behind a cost-guarded model router, on n8n clustered over Kubernetes. Two new metrics on Metabase so ops teams could act on it.

**Manual support escalations fell 40% in three months.**

#### Self-hosted analytics &nbsp;·&nbsp; rebuilt from zero

Google Analytics deleted the workspace with no warning and there was no budget for a commercial replacement. I reconstructed the event taxonomy, evaluated PostHog, Plausible, Openpanel and Rybbit against production traffic, **forked PostHog and patched its Next.js frontend and Python API** to spread load across ClickHouse clusters, then standardised on Rybbit under Coolify.

<br>

## Stack

| | |
| :--- | :--- |
| **Languages** | Python &nbsp;·&nbsp; TypeScript &nbsp;·&nbsp; Go &nbsp;·&nbsp; SQL |
| **Infrastructure** | Kubernetes &nbsp;·&nbsp; Ansible &nbsp;·&nbsp; WireGuard &nbsp;·&nbsp; AWS &nbsp;·&nbsp; Coolify &nbsp;·&nbsp; Traefik &nbsp;·&nbsp; Caddy |
| **Data** | ClickHouse &nbsp;·&nbsp; PostgreSQL &nbsp;·&nbsp; Redis &nbsp;·&nbsp; BigQuery &nbsp;·&nbsp; Metabase |
| **AI in production** | n8n &nbsp;·&nbsp; model routing with cost guardrails &nbsp;·&nbsp; RAG with vector embeddings |

These are tools I run and patch in production, not ones I only recommend. I operate them; I did not author them.

<br>

## Open source

I operate a lot of it, and contribute upstream when I hit a gap it makes sense to close.

<br>

---

<div align="center">
<sub>

Currently Head of Product Design, Quick Commerce at Digikala.<br>
Looking for forward deployed engineering and solutions work. Open to relocation.

</sub>
</div>
