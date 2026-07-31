---

title: "Week 6 Worklog"
date: 2026-07-18
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
----------------------

### Week 6 Objectives:

* Improve the response performance of the AI Face Recognition API by caching face embeddings in RAM.
* Strengthen the authentication mechanism by supporting both HttpOnly Cookies and Bearer Token headers as a fallback.
* Review and standardize the application's CORS configuration and Content Security Policy (CSP).

### Activities Breakdown:

| Day | Task Description                                                                                                                                            | Start Date | Completion Date |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- |
| Mon | - Improve `load_embeddings_into_cache()` to preload face vector embeddings into RAM when the application starts                                             | 13/07/2026 | 13/07/2026      |
| Tue | - Update `/auth/login` to provide the authentication `token` <br> - Configure `api.js` to send the token through the `Authorization: Bearer <token>` header | 14/07/2026 | 14/07/2026      |
| Wed | - Adjust the `connect-src` CSP directives in `index.html` and `backend/middleware/csp.py` <br> - Allow API communication across different domains           | 15/07/2026 | 15/07/2026      |
| Thu | - Update `DEV_ORIGINS` in `backend/main.py` <br> - Add the S3 Static Website domain to the list of permitted origins                                        | 16/07/2026 | 16/07/2026      |
| Fri | - Optimize the Vite production build using `manualChunks` <br> - Reduce the generated JavaScript bundle size to approximately 133 kB                        | 17/07/2026 | 19/07/2026      |

### Week 6 Deliverables:

* Improved Face Recognition API response time by loading face embeddings into RAM during application startup.
* Resolved cross-domain authentication issues between the S3-hosted Frontend and EC2 Backend.
* Reduced frontend bundle size and improved the overall Vite build performance.

