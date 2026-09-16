<p align="center">
  <img src="./assets/archive-header.svg" width="960" alt="DavidHLP — Engineering Archive. Java backend, caching and distributed systems." />
</p>

<p align="center">
  <a href="https://davidhlp.github.io/en">ARCHIVE TERMINAL</a> &nbsp; / &nbsp;
  <a href="https://github.com/DavidHLP?tab=repositories">SOURCE CODE</a> &nbsp; / &nbsp;
  <a href="#02--field-notes">FIELD NOTES</a>
</p>

## 00 / Profile

**Java backend developer working on caching and distributed systems.**

I maintain ResiCache and UltiCode. My work focuses on cache consistency, reliable asynchronous execution, and clear service boundaries. I write about the implementation details, trade-offs, and checks behind those systems.

> Correctness, clear boundaries, and reproducible results.

## 01 / Project index

### P–001 &nbsp; [ResiCache](https://github.com/DavidHLP/ResiCache)

**Composable cache protection for Spring Cache and Redis.**

Annotation-driven protection combines null-value caching, TTL jitter, distributed locking, and early refresh through a configurable handler chain. The engineering focus is explicit behavior around expiration, concurrent loading, and safe serialization.

<sub>JAVA &nbsp; / &nbsp; SPRING CACHE &nbsp; / &nbsp; REDIS &nbsp; / &nbsp; REDISSON</sub>

---

### P–002 &nbsp; [UltiCode](https://github.com/DavidHLP/UltiCode)

**An online judge platform with sandboxed code evaluation.**

Problem libraries, contests, and community features backed by application services and independent judge workers. A practical setting for service ownership, recoverable task delivery, and consistent API contracts.

<sub>JAVA &nbsp; / &nbsp; SPRING BOOT &nbsp; / &nbsp; REDIS &nbsp; / &nbsp; DOCKER &nbsp; / &nbsp; VUE</sub>

## 02 / Field notes

Selected implementation records. **Article text is in Chinese.**

| Record | Subject |
| :--- | :--- |
| `N–001` | [Cache stampedes: futures, distributed locks, and double-checking](https://davidhlp.github.io/note/resicache-single-flight) |
| `N–002` | [Recoverable judge delivery with an outbox and Redis Streams](https://davidhlp.github.io/note/ulticode-outbox-redis-streams) |

<p align="right"><a href="https://davidhlp.github.io/en">Explore the archive →</a></p>

---

<sub>DAVIDHLP &nbsp; / &nbsp; ENGINEERING ARCHIVE &nbsp; / &nbsp; PUBLIC INDEX</sub>
