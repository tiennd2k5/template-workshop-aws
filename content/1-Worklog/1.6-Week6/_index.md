---
title: "Week 6 Worklog"
date: 2026-07-17
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:
* Optimize AI Face Recognition API latency using RAM Cache embeddings.
* Enhance dual authentication strategy (HttpOnly Cookie + Bearer Token Header Fallback).
* Standardize CORS Whitelists and Content Security Policies (CSP).

### Activities Breakdown:
| Day | Task Description | Start Date | Completion Date |
| --- | --- | --- | --- |
| Mon | - Optimize `load_embeddings_into_cache()` loading face vectors directly into RAM during startup | 13/07/2026 | 13/07/2026 |
| Tue | - Return `token` in `/auth/login` and attach `Authorization: Bearer <token>` header in `api.js` | 14/07/2026 | 14/07/2026 |
| Wed | - Expand `connect-src` directives in `index.html` and `backend/middleware/csp.py` for cross-domain API calls | 15/07/2026 | 15/07/2026 |
| Thu | - Configure `DEV_ORIGINS` in `backend/main.py` adding S3 Static Web domain | 16/07/2026 | 16/07/2026 |
| Fri | - Optimize Vite frontend bundling with `manualChunks` reducing JS bundle size to 133 kB | 17/07/2026 | 19/07/2026 |

### Week 6 Deliverables:
* Significant latency drop in Face Recognition API responses due to RAM caching.
* Full cross-domain authentication fix between S3 Frontend and EC2 Backend.
* Optimized frontend bundle size and build performance.
