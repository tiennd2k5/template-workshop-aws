---
title: "Week 3 Worklog"
date: 2026-06-26
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:
* Launch EC2 Instance & configure Security Groups on AWS Console.
* Deploy Backend FastAPI Docker container onto EC2.
* Integrate AWS S3 storage for images, webcam logs & face vector embeddings (`boto3`).
* Deploy React/Vite Frontend onto AWS S3 Static Website Hosting.

### Activities Breakdown:
| Day | Task Description | Start Date | Completion Date |
| --- | --- | --- | --- |
| Mon | - Create AWS S3 Buckets for media storage & web hosting <br> - Integrate `boto3` SDK in `backend/services/s3_service.py` | 22/06/2026 | 23/06/2026 |
| Tue | - Save face registration & webcam log images directly to S3 | 24/06/2026 | 24/06/2026 |
| Wed | - Provision Ubuntu EC2 Instance, configure Security Group ports 80/8000/22 | 25/06/2026 | 25/06/2026 |
| Thu | - SSH to EC2, build & run `fav-web-backend` container with persistent Volume mounts | 26/06/2026 | 27/06/2026 |
| Fri | - Build `npm run build` pointing to EC2 Public IP and deploy to S3 Static Web | 28/06/2026 | 28/06/2026 |

### Week 3 Deliverables:
* Backend Docker running on AWS EC2 (`http://52.63.251.110`).
* Frontend React/Vite live on AWS S3 Static Website.
* Automatic S3 storage for uploaded images & face vector embeddings.

![AWS EC2 Instance Management](/images/ec2.png)
![AWS S3 Storage Management](/images/s3.png)
