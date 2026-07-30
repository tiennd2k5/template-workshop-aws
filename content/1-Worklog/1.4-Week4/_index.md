---
title: "Week 4 Worklog"
date: 2026-07-03
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:
* Provision and connect AWS RDS PostgreSQL Database (Free Tier).
* Configure Security Group rules between EC2 Backend and RDS PostgreSQL.
* Update SQLAlchemy `DATABASE_URL` supporting SQLite local and Cloud RDS PostgreSQL.
* Execute database seed scripts for initial admin user and default categories.

### Activities Breakdown:
| Day | Task Description | Start Date | Completion Date |
| --- | --- | --- | --- |
| Mon | - Provision AWS RDS PostgreSQL Instance via AWS Console | 29/06/2026 | 29/06/2026 |
| Tue | - Configure Security Group Inbound Rule allowing EC2 access on Port 5432 | 30/06/2026 | 30/06/2026 |
| Wed | - Add `psycopg2-binary` to `backend/requirements.txt` | 01/07/2026 | 01/07/2026 |
| Thu | - Update `backend/services/db_models.py` to parse `DATABASE_URL` dynamically from `.env` | 02/07/2026 | 03/07/2026 |
| Fri | - Test auto-migration and admin account seed (`123456`) on Cloud RDS | 04/07/2026 | 05/07/2026 |

### Week 4 Deliverables:
* EC2 Backend connected to AWS RDS PostgreSQL.
* Application data (Users, Posts, Knowledge, Games, Music, Logs) securely persisted on RDS.

![Online Music Streaming Module](/images/music.png)
![Game Blog News Module](/images/games.png)
![Multimedia Feed Module](/images/feed.png)
