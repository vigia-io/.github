<p align="center">
  <img src="https://raw.githubusercontent.com/vigia-io/.github/main/assets/vigia-org-banner.png" alt="Vigia — relational database observability" width="100%" />
</p>

# Vigia

**See your databases before incidents arrive.**

Vigia is a SaaS platform for observability across the relational databases your teams already run — SQL Server, MySQL, PostgreSQL, Oracle, and compatible engines.

We combine **offline-first collection** (a lightweight exporter inside your network) with a **multi-tenant cloud platform** for history, alerts, SLAs, and operational intelligence.

---

## How it works

```text
Your network                         Vigia Cloud
┌─────────────────┐                 ┌──────────────────┐
│ vigia-exporter  │  snapshot.json  │ Ingest API       │
│ (read-only SQL) │ ──────────────► │ History & alerts │
└────────┬────────┘                 │ Console & billing│
         │                          └──────────────────┘
         ▼
   SQL Server · MySQL · Azure SQL · PostgreSQL · Oracle
```

1. Run the exporter on a bastion or jump box — no inbound ports to your databases.
2. Upload signed snapshots to Vigia with your API key.
3. Monitor health, blocking, backups, capacity, and configuration drift from one console.

---

## Repositories

| Repository | Visibility | Purpose |
|------------|------------|---------|
| [**vigia-exporter**](https://github.com/vigia-io/vigia-exporter) | Public | Offline collection CLI |
| **vigia-spec** | Private | Product & architecture specification |
| **vigia-platform** | Private | API, ingest, multi-tenancy, billing |
| **vigia-console** | Private | Web dashboard |
| **vigia-scripts** | Private | Versioned SQL metric catalog |

---

## Licensing

| Component | Model |
|-----------|--------|
| **Exporter** | Public **source-available** code for audit — not MIT/Apache. [License](https://github.com/vigia-io/vigia-exporter/blob/main/LICENSE). Production use requires a Vigia account. |
| **Platform** | Commercial SaaS |

We are transparent where it builds trust (collection code) and commercial where we deliver ongoing value (platform, alerts, history, billing).

---

## Community

| Channel | Link |
|---------|------|
| Questions & feedback | [Open an issue](https://github.com/vigia-io/.github/issues) |
| Security reports | [SECURITY.md](https://github.com/vigia-io/.github/blob/main/SECURITY.md) |
| Contribution policy | [CONTRIBUTING.md](https://github.com/vigia-io/.github/blob/main/CONTRIBUTING.md) |

---

## Links

- **Website:** [getvigia.com](https://getvigia.com) *(coming soon)*
- **Exporter:** [github.com/vigia-io/vigia-exporter](https://github.com/vigia-io/vigia-exporter)
- **Contact:** legal@getvigia.com

<p align="center">
  <sub>Built for DBAs, SREs, and platform teams worldwide</sub>
</p>
