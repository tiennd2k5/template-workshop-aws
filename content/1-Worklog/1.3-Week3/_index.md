---

title: "Week 3 Worklog"
date: 2026-06-27
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
----------------------

### Week 3 Objectives:

* Set up an EC2 Instance and configure the required Security Group rules through the AWS Console.
* Deploy the FastAPI Backend as a Docker container on the EC2 environment.
* Connect the application to Amazon S3 for storing images, webcam logs, and face vector embeddings using `boto3`.
* Publish the React/Vite Frontend through Amazon S3 Static Website Hosting.

### Activities Breakdown:

| Day | Task Description                                                                                                                                                                         | Start Date | Completion Date |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- |
| Mon | - Set up S3 Buckets for application media files and frontend web hosting <br> - Connect the backend with S3 through the `boto3` SDK in `backend/services/s3_service.py`                  | 22/06/2026 | 23/06/2026      |
| Tue | - Modify the face registration and webcam logging process to upload image files directly to S3                                                                                           | 24/06/2026 | 24/06/2026      |
| Wed | - Create an Ubuntu EC2 Instance on AWS <br> - Configure Security Group access for ports 80, 8000, and 22                                                                                 | 25/06/2026 | 25/06/2026      |
| Thu | - Establish an SSH connection to the EC2 Instance <br> - Build and launch the `fav-web-backend` Docker container with persistent Volume mounts                                           | 26/06/2026 | 27/06/2026      |
| Fri | - Configure the frontend build using `npm run build` with the EC2 Public IP as the backend endpoint <br> - Upload and deploy the generated React/Vite files to S3 Static Website Hosting | 28/06/2026 | 28/06/2026      |

### Week 3 Deliverables:

* FastAPI Backend successfully running inside a Docker container on AWS EC2.
* React/Vite Frontend deployed and accessible through AWS S3 Static Website Hosting.
* Uploaded images and face vector embeddings automatically stored in Amazon S3.



