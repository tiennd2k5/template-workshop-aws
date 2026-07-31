---

title: "Week 4 Worklog"
date: 2026-07-05
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
----------------------

### Week 4 Objectives:

* Set up an AWS RDS PostgreSQL database and establish the connection with the application.
* Configure the necessary Security Group rules to allow communication between the EC2 Backend and RDS PostgreSQL.
* Modify the SQLAlchemy database configuration to support both the local SQLite database and the PostgreSQL database hosted on AWS RDS.
* Prepare and run database seed scripts to create the initial administrator account and default application categories.

### Activities Breakdown:

| Day | Task Description                                                                                                                                                                                           | Start Date | Completion Date |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- |
| Mon | - Create and configure a PostgreSQL database instance using AWS RDS through the AWS Console                                                                                                                | 29/06/2026 | 29/06/2026      |
| Tue | - Adjust the RDS Security Group configuration <br> - Allow inbound PostgreSQL connections from the EC2 Backend through Port 5432                                                                           | 30/06/2026 | 30/06/2026      |
| Wed | - Install the PostgreSQL Python driver by adding `psycopg2-binary` to `backend/requirements.txt`                                                                                                           | 01/07/2026 | 01/07/2026      |
| Thu | - Modify `backend/services/db_models.py` to read and process the `DATABASE_URL` configuration dynamically from `.env` <br> - Maintain compatibility between local SQLite and cloud PostgreSQL environments | 02/07/2026 | 03/07/2026      |
| Fri | - Verify database auto-migration on the cloud environment <br> - Run the seed process to initialize the administrator account (`123456`) and required default data on RDS                                  | 04/07/2026 | 05/07/2026      |

### Week 4 Deliverables:

* Successfully establish a connection between the FastAPI Backend running on EC2 and the PostgreSQL database hosted on AWS RDS.
* Application data, including Users, Posts, Knowledge, Games, Music, and Logs, is stored persistently on the RDS database.

