---

title: "Week 5 Worklog"
date: 2026-07-11
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
----------------------

### Week 5 Objectives:

* Set up centralized application logging using AWS CloudWatch Logs.
* Establish monitoring rules, metric filters, and alarms for the EC2 instance and Backend services.

### Activities Breakdown:

| Day | Task Description                                                                                                                                                         | Start Date | Completion Date |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- |
| Mon | - Explore AWS CloudWatch Logs and understand its role in application monitoring <br> - Study the usage of the `watchtower` Python logging library                        | 06/07/2026 | 06/07/2026      |
| Tue | - Include `watchtower` in `backend/requirements.txt` <br> - Update the logging implementation in `backend/services/logging_service.py`                                   | 07/07/2026 | 08/07/2026      |
| Thu | - Configure application logs to be forwarded to the CloudWatch Log Group `/fav-web/backend` <br> - Monitor Face ID events, login activities, and database-related errors | 09/07/2026 | 10/07/2026      |
| Sat | - Create a CloudWatch Alarm for the EC2 instance <br> - Configure the alarm to trigger when CPU utilization goes above 80%                                               | 11/07/2026 | 12/07/2026      |

### Week 5 Deliverables:

* Application logs are automatically collected from the EC2 Backend and forwarded to AWS CloudWatch.
* EC2 CPU usage monitoring and the corresponding CloudWatch alarm are successfully configured.



