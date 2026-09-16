# David

**Java Backend Developer · Caching & Distributed Systems**

I build Java backend systems and open-source tools, with a focus on cache consistency, reliable asynchronous execution, and clear service boundaries.
This is where I share the projects I maintain and the engineering decisions behind them.

[Writing](https://davidhlp.github.io/) · [Repositories](https://github.com/DavidHLP?tab=repositories)

## Selected projects

### [ResiCache](https://github.com/DavidHLP/ResiCache)

Composable cache protection for Spring Cache and Redis.

- Combines null-value caching, TTL jitter, distributed locking, and early refresh through annotations and a configurable handler chain.
- Focuses on explicit, testable behavior around cache expiration, concurrent loading, and safe serialization.

`Java` · `Spring Cache` · `Redis` · `Redisson`

### [UltiCode](https://github.com/DavidHLP/UltiCode)

An online judge platform for programming problems, contests, sandboxed evaluation, and community discussions.

- Separates application services from sandboxed judge workers, with asynchronous submission processing and result delivery.
- Explores service ownership, failure recovery, and consistent API contracts across backend and frontend applications.

`Java` · `Spring Boot` · `Redis` · `Docker` · `Vue` · `TypeScript`

## Engineering notes

Implementation details, trade-offs, and verification notes. Articles below are in Chinese.

- [Cache stampedes: why combine futures, distributed locks, and double-checking?](https://davidhlp.github.io/note/resicache-single-flight)
- [Recoverable judge delivery with an outbox and Redis Streams](https://davidhlp.github.io/note/ulticode-outbox-redis-streams)

---

<sub>Correctness, clear boundaries, and reproducible results.</sub>
