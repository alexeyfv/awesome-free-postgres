# 🐘 Awesome Free PostgreSQL as a Service

A curated list of **free PostgreSQL as a Service** (PaaS) providers. Ideal for hobby projects, prototypes, learning, and experiments.

## ❓ Why This List?

PostgreSQL is a powerful open-source relational database — but running it in the cloud can cost money.  
Luckily, several cloud providers offer **free-tier** PostgreSQL services.

This repo helps developers discover and compare these options in one place.

## 📌 Inclusion Criteria

To be included in this list, a PostgreSQL provider must meet all of the following:

- **Free registration** and **no credit card required**.
- **No time limits** on usage of the free tier — i.e., you can run your DB 24/7 without auto-deletion after a fixed trial period.

## 📊 Comparison

### 🔧 Core Specs

| Provider                                                                                                         | Space      | CPU     | RAM     | Backups                                                                                                                                                                                 |
| ---------------------------------------------------------------------------------------------------------------- | ---------- | ------- | ------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [aiven.io](https://aiven.io/docs/platform/concepts/free-plan)                                                    | 1 GB       | 1       | 1 GB    | [Daily backups](https://aiven.io/docs/products/postgresql/concepts/pg-backups). Restore is [paid-only](https://aiven.io/community/forum/t/how-do-i-get-mysql-backup-in-free-tier/1127). |
| [filess.io](https://filess.io)                                                                                   | 2 × 10 MB  | N/A     | N/A     | Weekly backups                                                                                                                                                                          |
| [mkdb.sh](https:/mkdb.sh)                                                                                        | 10 × 20 MB | N/A     | N/A     | ❌                                                                                                                                                                                       |
| [supabase.com](https://supabase.com)                                                                             | 500 MB     | N/A     | 500 MB  | ❌                                                                                                                                                                                       |
| [prisma.io](https://prisma.io/pricing)                                                                           | 500 MB     | N/A     | N/A     | ❌                                                                                                                                                                                       |
| [nhost.io](https://nhost.io/)                                                                                    | 1 GB       | 0.5 CPU | 256 MiB | ❌                                                                                                                                                                                       |
| [tigerdata.com](https://www.tigerdata.com/blog/introducing-agentic-postgres-free-plan-experiment-ai-on-postgres) | 2 x 750 MB | N/A     | N/A     | 24h PITR                                                                                                                                                                                |
| [rivestack.io](https://docs.rivestack.io/pricing) \*\*                                                                                                   | 2 GB       | N/A     | N/A     | ❌                                                                                                                                                            |
\*\* **Rivestack** comes with the [pgvector](https://github.com/pgvector/pgvector) extension pre-installed on all databases, including the free tier.

### 🛑 Limits

> ℹ️ All limits below are applied **monthly**, unless stated otherwise.

| Provider                                                                                                         | Network                    | Other Limits         | Pause Policy                                                                                                                                       |
| ---------------------------------------------------------------------------------------------------------------- | -------------------------- | -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| [aiven.io](https://aiven.io)                                                                                     | —                          | —                    | [Shuts down after inactivity; exact duration not specified](https://aiven.io/docs/platform/concepts/free-plan#free-plan-features-and-limitations). |
| [filess.io](https://filess.io)                                                                                   | —                          | —                    | No pause                                                                                                                                           |
| [mkdb.sh](https://mkdb.sh)                                                                                       | —                          | —                    | No pause                                                                                                                                           |
| [supabase.com](https://supabase.com)                                                                             | 5 GB                       | —                    | [May pause after 7 days of low activity](https://supabase.com/docs/guides/deployment/going-into-prod#availability).                                |
| [prisma.io](https://prisma.io/pricing)                                                                           | 100,000 operations / month | —                    | No pause                                                                                                                                           |
| [nhost.io](https://nhost.io/)                                                                                    | 5 GB egress                | 1 project, 1 memeber | [Paused after 1 week inactivity](https://nhost.io/pricing)                                                                                         |
| [tigerdata.com](https://www.tigerdata.com/blog/introducing-agentic-postgres-free-plan-experiment-ai-on-postgres) | —                          | —                    | No pause                                                                                                                                           |
| [rivestack.io](https://rivestack.io)                                                                             | —                          | 1 database, 5 connections | No pause                                                                                                                                      |

### 🌍 Regions & Registration

| Provider                                                                                                     | Registration                     | Locations                       |
| ------------------------------------------------------------------------------------------------------------ | -------------------------------- | ------------------------------- |
| [aiven.io](https://aiven.io)                                                                                 | Email, Google, GitHub, Microsoft | US, Europe, Asia, South America |
| [filess.io](https://filess.io) \*                                                                            | Email, Google                    | US, Europe, Asia                |
| [mkdb.sh](https://mkdb.sh)                                                                                   | GitHub                           | US, Europe, Asia                |
| [supabase.com](https://supabase.com)                                                                         | Email, GitHub                    | US, Europe, Asia                |
| [prisma.io](https://prisma.io/docs/postgres/more/faq#what-regions-is-prisma-postgres-available-in)           | GitHub, Google, Email            | US, Europe, Asia                |
| [nhost.io](https://nhost.io/)                                                                                | GitHub, Email                    | US, Europe, Asia, South America |
| [tigerdata.com](https://tigerdata.com/blog/introducing-agentic-postgres-free-plan-experiment-ai-on-postgres) | Google, Email                    | US                              |
| [rivestack.io](https://rivestack.io)                                                                        | Email, Google, GitHub            | US, Europe                      |

\* **Filess** automatically selects a region based on your location. In my case, it was Nuremberg with no way to change the region manually.

## 🤝 Contributing

Found a new service? Something outdated or inaccurate?

Check out [CONTRIBUTING.md](CONTRIBUTING.md) for how to contribute.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=alexeyfv/awesome-free-postgres&type=Date)](https://www.star-history.com/#alexeyfv/awesome-free-postgres&Date)
