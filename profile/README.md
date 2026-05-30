# System Design Series

> **Real-world system design problems, studied end-to-end — each with a full design write-up _and_ runnable code.**

Most system-design resources stop at boxes-and-arrows. This series goes further: every topic ships a written design (requirements → estimation → API → architecture → data model → deep dives → trade-offs) **alongside a working implementation** you can run, read, and break. Built for **system design interview preparation**, for learning **distributed systems** and **scalability** patterns, and for anyone who learns best from code that actually runs.

![Topics](https://img.shields.io/badge/topics-1-blue)
![Focus](https://img.shields.io/badge/focus-distributed%20systems%20%C2%B7%20scalability-6f42c1)
![Code](https://img.shields.io/badge/every%20topic-design%20%2B%20runnable%20code-success)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 📚 Topics

| # | Topic | Problem | Core ideas | Stack |
|---|-------|---------|-----------|-------|
| 1 | **[fb-live-comments](https://github.com/system-design-series/fb-live-comments)** | Live-video comment section (FB/IG Live): post + read comments in near-real-time at viewer scale | Sharded pub/sub fan-out · SSE live tail · recent-window cache · read-your-own-writes · keyset pagination · gap-free reconnect | Go · Postgres · Redis Cluster |

*More topics are added over time. Each is a standalone repository in this org.*

## 🧭 How each topic is organized

Every topic is its **own repository** under this org, with a consistent layout:

```
<topic>/
├── README.md   # the "what" + how to run it
├── DESIGN.md   # the "why" — full high-level design write-up
└── <code>      # runnable implementation (services, infra, frontend)
```

Start with `DESIGN.md` for the reasoning, then `README.md` to run it.

## 🤖 For AI agents & programmatic readers

This org is structured to be easy to navigate without a human in the loop:

- **One topic = one repository.** List them via the GitHub API: `GET /orgs/system-design-series/repos`.
- **Predictable files per repo:** `README.md` (overview + run steps), `DESIGN.md` (architecture & trade-offs), and source under conventional paths.
- **Discoverable by topic tags:** each repo is labeled with GitHub topics (e.g. `system-design`, `distributed-systems`, `scalability`) for search and filtering.
- **Self-contained:** no cross-repo build dependencies — each topic runs on its own.

## 🛠️ Concepts covered across the series

`system design` · `distributed systems` · `scalability` · `high availability` · `caching` · `sharding` · `pub/sub & fan-out` · `real-time delivery (SSE / WebSockets)` · `data modeling` · `pagination` · `consistency & trade-offs` · `capacity estimation` · `system design interview prep`

## 🤝 Contributing & feedback

Issues and discussions on any repo are welcome — corrections, alternative designs, and "why not X?" questions make the write-ups better. Each repo is **MIT-licensed**: learn from it, fork it, build on it.
