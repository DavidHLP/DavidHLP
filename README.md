![Engineering Archive — a personal engineering index](assets/archive-header.svg)

# DavidHLP

**Java Backend Developer**

I build Java backend services and reusable components, focusing on cache behavior, asynchronous execution, and service boundaries. My work also spans frontend integration and AI-assisted full-stack development.

[Blog](https://davidhlp.github.io/) · [Projects](#01--selected-projects) · [Notes](#03--field-notes) · [简体中文](README.zh-CN.md)

## 01 / Selected Projects

### [ResiCache](https://github.com/DavidHLP/ResiCache)

A Spring Cache extension for composing Redis cache protection.

- **Composable policies.** An ordered, configurable handler chain separates protection rules from cache operations.
- **Concurrent loading.** With `sync=true`, same-key callers within one JVM share a loading result; cross-instance coordination requires a distributed-lock backend.

**Stack:** Java · Spring Cache · Redis · Redisson

Early-stage; APIs may change. The main branch targets Spring Boot 4 / Java 21; check compatibility before choosing a published release.

[Loading implementation](https://github.com/DavidHLP/ResiCache/blob/main/src/main/java/io/github/davidhlp/spring/cache/redis/cache/SyncSupport.java) · [Compatibility & limitations](https://github.com/DavidHLP/ResiCache/blob/main/COMPATIBILITY.md)

---

### [UltiCode](https://github.com/DavidHLP/UltiCode)

An online judge platform for submitting code and evaluating it against test cases.

- **Task delivery.** The outbox path feeds Redis Streams, with retries for dispatch failures and dead-letter handling for malformed jobs.
- **Execution boundary.** Independent judge workers run submitted code in Docker with network isolation and CPU, memory, and process limits.

**Stack:** Java · Spring Boot · Redis · Docker · Vue 3 · TypeScript

The Core profile is an opt-in architecture experiment, not the default topology. The project has no production environment.

[Delivery implementation](https://github.com/DavidHLP/UltiCode/blob/main/services/submission/src/main/java/com/ulticode/modules/queue/outbox/dispatcher/JudgeOutboxDispatcher.java) · [Project status & boundaries (Chinese)](https://github.com/DavidHLP/UltiCode/blob/main/docs/project/current-status.md)

## 02 / Engineering Approach

I start from explicit contracts and failure cases, and check changes with focused tests, logs, and reproducible steps. I write and debug code independently, using AI to assist exploration and implementation while reviewing its output myself.

## 03 / Field Notes

Selected implementation notes. **Both articles are in Chinese; original titles are retained.**

- [缓存击穿时，为什么要同时有 Future、分布式锁和 double-check？](https://davidhlp.github.io/note/resicache-single-flight/) — Request coalescing, lock scope, and failure propagation.
- [UltiCode Outbox 与 Redis Streams：把判题投递做成可恢复状态](https://davidhlp.github.io/note/ulticode-outbox-redis-streams/) — Durable delivery intent, retries, and recovery boundaries.

[More writing on the blog →](https://davidhlp.github.io/)
