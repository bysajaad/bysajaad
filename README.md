<div align="center">

# Sajad Roudbari

**`Forward Deployed Engineer`** &nbsp;•&nbsp; **`Solutions Architect`**

<samp>I get access. I ship. I keep it running.</samp>

<br>

[![Website](https://img.shields.io/badge/iamsajaad.com-0D1117?style=for-the-badge&logo=safari&logoColor=58A6FF&labelColor=0D1117)](https://iamsajaad.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0D1117?style=for-the-badge&logo=linkedin&logoColor=58A6FF&labelColor=0D1117)](https://linkedin.com/in/iamsajaad)
[![Email](https://img.shields.io/badge/hi@iamsajaad.com-0D1117?style=for-the-badge&logo=maildotru&logoColor=58A6FF&labelColor=0D1117)](mailto:hi@iamsajaad.com)

<sub>📍 Tehran, Iran &nbsp;·&nbsp; ✈️ Open to relocation &nbsp;·&nbsp; 🗣️ Persian · English</sub>

</div>

---

> [!NOTE]
> **I go into messy environments, get access, ship working systems end to end, and then run them in production.**
> Analytics platforms, LLM pipelines, payment integrations. Most of what I have shipped started as a problem nobody owned, with no mandate to fix it.

<br>

## 🧠 &nbsp;Call intelligence at Digikala

Quality control ran on a **random 10% sample** of call-centre calls, and escalation was how anything outside that sample got found. I negotiated archive access out of the company's most regulation-bound data team, then built a pipeline over the **full daily volume**.

```mermaid
flowchart LR
    A["Call archive<br/>full daily volume"] --> B["Transcription"]
    B --> C["Index"]
    C --> D["Sentiment"]
    C --> E["Compliance<br/>flagging"]
    D --> F["Metabase<br/>NSS + severity index"]
    E --> F
    E --> G["Auto-route to<br/>account mgmt / commercial / sales"]
    C --> H["RAG over<br/>vector embeddings"]
```

<table>
<tr>
<td width="33%" align="center"><h3>−40%</h3><sub>manual support escalations<br/>in three months</sub></td>
<td width="33%" align="center"><h3>10% → 100%</h3><sub>call coverage<br/>replacing random sampling</sub></td>
<td width="33%" align="center"><h3>2</h3><sub>new metrics ops teams<br/>now run on</sub></td>
</tr>
</table>

<sub>`n8n on Kubernetes` · `cost-guarded model router` · `ClickHouse` · `Metabase` · `Python`</sub>

<br>

## 📡 &nbsp;Zonerift &nbsp;<sub><sup>built and operated solo</sup></sub>

Most privacy tools push all traffic through one exit IP, so you trade speed for reach. This one decides **per service**, and switches mid-session without dropping the connection.

```mermaid
flowchart LR
    U["User session"] --> R{"Service-aware<br/>router"}
    R -->|"streaming"| A["US region"]
    R -->|"latency-sensitive"| B["Nearest region"]
    R -->|"crypto"| C["East Asia region"]
```

<table>
<tr>
<td width="33%" align="center"><h3>~1.5 PB</h3><sub>per month</sub></td>
<td width="33%" align="center"><h3>99.9%</h3><sub>uptime, effectively<br/>unattended</sub></td>
<td width="33%" align="center"><h3>18</h3><sub>AWS regions<br/>via Ansible</sub></td>
</tr>
</table>

<details>
<summary><b>How it holds together</b></summary>

<br>

WireGuard across 18 AWS regions, provisioned with Ansible so every region stays in sync from one source of truth. PostgreSQL for accounts, Redis for licence checks and live usage, both behind a Python REST API.

Billing has no third-party provider: **10+ fiat and crypto rails**, plus a Telegram bot handling subscriptions and renewals. Health and status through uptime kuma and instatus.

AWS funded the first year of infrastructure.

</details>

<sub>`WireGuard` · `Ansible` · `AWS` · `PostgreSQL` · `Redis` · `Python` · `Traefik`</sub>

<br>

## 📊 &nbsp;Self-hosted analytics, rebuilt from zero

Google Analytics deleted the workspace with no warning, and there was no budget for a commercial replacement.

```
     event taxonomy         →  reconstructed from scratch
     4 platforms            →  tested against production traffic
     PostHog                →  forked, patched, load spread over ClickHouse
     Rybbit under Coolify   →  where it landed
```

<sub>`ClickHouse` · `Next.js` · `Python` · `BigQuery` · `Coolify` · `Rybbit`</sub>

<br>

## ⚙️ &nbsp;Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![WireGuard](https://img.shields.io/badge/WireGuard-88171A?style=flat-square&logo=wireguard&logoColor=white)
![Traefik](https://img.shields.io/badge/Traefik-24A1C1?style=flat-square&logo=traefikproxy&logoColor=white)

![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=flat-square&logo=clickhouse&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?style=flat-square&logo=googlebigquery&logoColor=white)
![Metabase](https://img.shields.io/badge/Metabase-509EE3?style=flat-square&logo=metabase&logoColor=white)

![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white)
![Coolify](https://img.shields.io/badge/Coolify-8B5CF6?style=flat-square&logo=coolify&logoColor=white)
![PostHog](https://img.shields.io/badge/PostHog-F54E00?style=flat-square&logo=posthog&logoColor=white)

</div>

> [!IMPORTANT]
> These are tools I **run and patch in production**, not ones I only recommend. I operate them. I did not author them.

<br>

## 🌱 &nbsp;Open source

I operate a lot of it, and contribute upstream when I hit a gap worth closing.

<br>

---

<div align="center">
<sub>

Head of Product Design, Quick Commerce **@ Digikala** &nbsp;·&nbsp; Founder **@ Zonerift**

Looking for forward deployed engineering and solutions work.

</sub>
</div>
