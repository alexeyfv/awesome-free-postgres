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

| Provider                             | Space      | CPU      | RAM    | Backups                                                                                                                                                                                 |
| ------------------------------------ | ---------- | -------- | ------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [aiven.io](https://aiven.io)         | 1 GB       | 2        | 1 GB   | [Daily backups](https://aiven.io/docs/products/postgresql/concepts/pg-backups). Restore is [paid-only](https://aiven.io/community/forum/t/how-do-i-get-mysql-backup-in-free-tier/1127). |
| [filess.io](https://filess.io)       | 2 × 10 MB  | N/A      | N/A    | Weekly backups                                                                                                                                                                          |
| [mkdb.sh](https://www.mkdb.sh)       | 10 × 20 MB | N/A      | N/A    | ❌                                                                                                                                                                                       |
| [neon.tech](https://neon.tech) *     | 500 MB     | 0.25 – 2 | 1 GB   | [PITR for 24 hours](https://neon.tech/docs/manage/backups)                                                                                                                              |
| [supabase.com](https://supabase.com) | 500 MB     | N/A      | 500 MB | ❌                                                                                                                                                                                       |
| [xata.io](https://lite.xata.io/)     | 15 GB      | N/A      | N/A    | [Daily backups. Restoration is available once per month](https://xata.io/docs/concepts/pricing#daily-backups)                                                                          |

\* **Neon** has auto-scaling enabled by default. It's recommended to disable it to avoid exceeding the 190 compute hours/month quota.

### 🛑 Limits

> ℹ️ All limits below are applied **monthly**, unless stated otherwise.

| Provider                             | Network                                                                                                                                                  | Other Limits           | Pause Policy                                                                                                                                                                          |
| ------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [aiven.io](https://aiven.io)         | —                                                                                                                                                        | —                      | [Shuts down after inactivity; exact duration not specified](https://aiven.io/docs/platform/concepts/free-plan#free-plan-features-and-limitations).                                    |
| [filess.io](https://filess.io)       | —                                                                                                                                                        | —                      | No pause                                                                                                                                                                              |
| [mkdb.sh](https://www.mkdb.sh)       | —                                                                                                                                                        | —                      | No pause                                                                                                                                                                              |
| [neon.tech](https://neon.tech)       | 5 GB                                                                                                                                                     | 190 compute hours      | [Auto pause after 5 minutes of inactivity (cannot be disabled on free plan)](https://neon.tech/docs/guides/scale-to-zero-guide).                                                      |
| [supabase.com](https://supabase.com) | 5 GB                                                                                                                                                     | —                      | [May pause after 7 days of low activity](https://supabase.com/docs/guides/deployment/going-into-prod#availability).                                                                   |
| [xata.io](https://lite.xata.io/)     | [Concurrency limits](https://xata.io/docs/concepts/pricing#concurrency-limit), [Requests rate limits](https://xata.io/docs/concepts/pricing#rate-limit). | -                      | [Marked as inactive if there is no activity registered within 30 days](https://xata.io/docs/inactive-branches)                                                                        |

### 🌍 Regions & Registration

| Provider                             | Registration                     | Locations                                                                       |
| ------------------------------------ | -------------------------------- | ------------------------------------------------------------------------------- |
| [aiven.io](https://aiven.io)         | Email, Google, GitHub, Microsoft | US, Europe, Asia, South America                                                 |
| [filess.io](https://filess.io) *     | Email, Google                    | US, Europe, Asia                                                                |
| [mkdb.sh](https://www.mkdb.sh)       | GitHub                           | US, Europe, Asia                                                                |
| [neon.tech](https://neon.tech)       | Email, Google, GitHub, Microsoft | US, Canada, Europe, Asia                                                        |
| [supabase.com](https://supabase.com) | Email, GitHub                    | US, Europe, Asia                                                                |
| [xata.io](https://lite.xata.io/)     | Email, Google, GitHub            | [US, Europe, Australia](https://xata.io/docs/getting-started/available-regions) |

\* **Filess** automatically selects a region based on your location. In my case, it was Nuremberg with no way to change the region manually.

## 🤝 Contributing

Found a new service? Something outdated or inaccurate?

Check out [CONTRIBUTING.md](CONTRIBUTING.md) for how to contribute.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=alexeyfv/awesome-free-postgres&type=Date)](https://www.star-history.com/#alexeyfv/awesome-free-postgres&Date)
