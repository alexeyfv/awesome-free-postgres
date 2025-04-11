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

## 📊 Comparison Table

| Provider                             | Registration                     | Space      | CPU      | RAM    | Network | Other Limits            | Backups                                                                                                                                                                                 | Locations                                        |
| ------------------------------------ | -------------------------------- | ---------- | -------- | ------ | ------- | ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ |
| [tembo.io](https://tembo.io)         | Email, GitHub, Google            | 10 GB      | 0.25     | 1 GB   | —       | —                       | [PITR for 24 hours](https://tembo.io/docs/product/cloud/configuration-and-management/backup-and-restore)                                                                                | US, Canada, Europe, Asia, Oceania, South America |
| [turso.tech](https://turso.tech)     | Email, Google, GitHub            | 5 GB       | N/A      | 1 GB   | 5 GB    | 500M reads, 10M writes  | [PITR for 24 hours](https://docs.turso.tech/features/point-in-time-recovery)                                                                                                            | US, Europe, Asia                                 |
| [neon.tech](https://neon.tech) *     | Email, Google, GitHub, Microsoft | 500 MB     | 0.25 – 2 | 1 GB   | 5 GB    | 190 compute hours/month | [PITR for 24 hours](https://neon.tech/docs/manage/backups)                                                                                                                              | US, Canada, Europe, Asia                         |
| [aiven.io](https://aiven.io)         | Email, Google, GitHub, Microsoft | 5 GB       | 2        | 1 GB   | —       | —                       | [Daily backups](https://aiven.io/docs/products/postgresql/concepts/pg-backups). Restore is [paid-only](https://aiven.io/community/forum/t/how-do-i-get-mysql-backup-in-free-tier/1127). | US, Europe, Asia, South America                  |
| [filess.io](https://filess.io) **    | Email, Google                    | 2 × 10 MB  | N/A      | N/A    | —       | —                       | Weekly backups.                                                                                                                                                                          | US, Europe, Asia                                 |
| [supabase.com](https://supabase.com) | Email, GitHub                    | 500 MB     | N/A      | 500 MB | 5 GB    | —                       | ❌                                                                                                                                                                                       | US, Europe, Asia                                 |
| [mkdb.sh](https://www.mkdb.sh)       | GitHub                           | 10 × 20 MB | N/A      | N/A    | —       | —                       | ❌                                                                                                                                                                                       | US, Europe, Asia                                 |

\* Neon has auto-scaling enabled by default. It's recommended to disable it to avoid exceeding the 190 compute hours/month quota.

\** Filess automatically selects a region based on your location. In my case, it was Nuremberg with no way to change the region manually.

## 🤝 Contributing

Found a new service? Something outdated or inaccurate?

Check out [CONTRIBUTING.md](CONTRIBUTING.md) for how to contribute.
