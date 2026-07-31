---

title: "Week 7 Worklog"
date: 2026-07-25
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
----------------------

### Week 7 Objectives:

* Conduct end-to-end validation of the application across the AWS S3 Frontend and EC2 Backend environments.
* Verify the system's ability to handle failures caused by database disconnection and network latency.
* Evaluate the user experience of webcam-based face scanning and media streaming features.

### Activities Breakdown:

| Day | Task Description                                                                                                                                 | Start Date | Completion Date |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- |
| Mon | - Perform E2E tests covering account registration, Face ID authentication, Feed posts, and Bookmarks                                             | 20/07/2026 | 21/07/2026      |
| Wed | - Measure frontend page loading time under actual network conditions <br> - Check the response speed and stability of the webcam face scanner    | 22/07/2026 | 23/07/2026      |
| Fri | - Test application error handling and recovery mechanisms <br> - Verify system responses to Rate Limit `429` and expired Session `401` scenarios | 24/07/2026 | 26/07/2026      |

### Week 7 Deliverables:

* Core application workflows between the AWS S3 Frontend and EC2 Backend operate reliably and consistently.
* Error handling, recovery mechanisms, and user feedback are functioning as expected.

