---
title: "Week 5 Worklog"
date: 2026-07-10
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:
* Integrate application logging with AWS CloudWatch Logs.
* Configure metric filters & alarms for EC2 instance and Backend services.

### Activities Breakdown:
| Day | Task Description | Start Date | Completion Date |
| --- | --- | --- | --- |
| Mon | - Research AWS CloudWatch Logs service & `watchtower` Python SDK | 06/07/2026 | 06/07/2026 |
| Tue | - Add `watchtower` to `backend/requirements.txt` and update `backend/services/logging_service.py` | 07/07/2026 | 08/07/2026 |
| Thu | - Configure log streaming for Face ID events, logins, and DB errors to CloudWatch Log Group `/fav-web/backend` | 09/07/2026 | 10/07/2026 |
| Sat | - Provision CloudWatch Alarm triggering when EC2 CPU utilization exceeds 80% | 11/07/2026 | 12/07/2026 |

### Week 5 Deliverables:
* Automatic application log streaming from EC2 to AWS CloudWatch.
* CPU utilization monitoring & alarm system operational.

![AWS CloudWatch Logging & Monitoring](/images/cloudwatch.png)
