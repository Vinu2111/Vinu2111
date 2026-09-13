<h1 align="center">Vinayak Gote</h1>
<h3 align="center">Java Backend Engineer · OSS Contributor (Zalando · Adyen · Picnic · Debezium · Kestra) · NVIDIA AI Aerial / 6G Developer Program</h3>

<p align="center">
  <a href="https://linkedin.com/in/vinayakgote">LinkedIn</a> &nbsp;·&nbsp;
  <a href="https://github.com/Vinu2111">GitHub</a> &nbsp;·&nbsp;
  <a href="https://vinayak6g.hashnode.dev">Blog</a> &nbsp;·&nbsp;
  <a href="https://dev.to/vinayakgote">Dev.to</a> &nbsp;·&nbsp;
  <a href="mailto:vinayakgote44@gmail.com">Email</a> &nbsp;·&nbsp;
  <a href="https://portfolio-gules-ten-40.vercel.app">Portfolio</a>
</p>

<br/>

Backend engineer at **Wipro**, building production REST APIs for VodafoneIdea telecom systems with Spring Boot 3. My strategy for breaking into product companies I respect: contribute real code to their OSS repos before applying. That's led to **6 merged PRs** across Zalando, Adyen, and Picnic, with **8 open PRs** in active review across 5 organizations including Debezium, NVlabs, and Kestra.

Member of the **NVIDIA AI Aerial / 6G Developer Program** after bug fixes in the Sionna SDK, with a public mention from NVIDIA core maintainer Merlin Nimier-David.

I write daily on [Hashnode](https://vinayak6g.hashnode.dev) and [Dev.to](https://dev.to/vinayakgote) backend engineering, OSS learnings, and Java deep-dives.

---

## 🟢 Currently

- Landed a Refaster rule in **Picnic/error-prone-support** (#2275) — rewrites `Optional.of(x).orElse(y)` to `requireNonNull(x)`, approach approved by Stephan202
- New PR in review at **Picnic/error-prone-support** (#2291) — `CollectorMutability`, replacing manual mutable-collector patterns with JDK-native unmodifiable collectors
- Opened **zalando/logbook** #2385 (colored pretty-printing for local dev via `AnsiPrettyPrintingSink`) and #2386 (new `logbook-jdkhttpclient` module adding `java.net.http.HttpClient` support)
- Opened two PRs on **kestra-io/kestra** — #19081 (fixes a UID-collision bug in `IdUtils.fromParts`) and #19219 (preserves title/description on a retry type discriminator field)
- Debezium PostgreSQL connector fix (#7462) — under active review with core maintainers
- Building [`picnic-store-intelligence`](https://github.com/Vinu2111/picnic-store-intelligence) — an architectural prototype exploring Picnic's Page Platform philosophy (server-driven layouts + per-customer section ranking)
- Self-studying German toward Goethe-Institut certification

---

## 🤝 Open Source Contributions

### ✅ Merged — 6 PRs

| # | Org | Repository | What I did |
|---|---|---|---|
| 1 | **Zalando** | [zalando/logbook #2301](https://github.com/zalando/logbook/pull/2301) | Implemented `StatusCodeBasedSink` + `LevelBasedHttpLogWriter` — HTTP status-code-aware log levels (2xx/3xx → TRACE, 4xx → WARN, 5xx → ERROR) |
| 2 | **Zalando** | [zalando/logbook #2326](https://github.com/zalando/logbook/pull/2326) | Fixed JSON formatter embedding non-JSON bodies (ciphertext/binary) as invalid, unquoted JSON |
| 3 | **Zalando** | [zalando/logbook #2327](https://github.com/zalando/logbook/pull/2327) | Wrapped `LogbookClientHttpRequestInterceptor` bean registration in a `@ConditionalOnClass` guard — fixed a startup crash in environments without spring-web |
| 4 | **Zalando** | [zalando/logbook #2328](https://github.com/zalando/logbook/pull/2328) | Fixed `CachingHttpResponse` dropping attributes when `withoutBody()` is called |
| 5 | **Adyen** | [adyen/adyen-java-api-library #1952](https://github.com/Adyen/adyen-java-api-library/pull/1952) | Fixed unescaped regex dots in `Service.createBaseURL` — shipped in **SDK v42.0.0** |
| 6 | **Picnic** | [error-prone-support #2275](https://github.com/PicnicSupermarket/error-prone-support/pull/2275) | Refaster rule: rewrites `Optional.of(x).orElse(y)` dead-code anti-pattern → `requireNonNull(x)`. Approach approved by Stephan202 |

### ⏳ Open — 8 PRs in active review

| # | Org | Repository | What I did |
|---|---|---|---|
| 7 | **Picnic** | [error-prone-support #2291](https://github.com/PicnicSupermarket/error-prone-support/pull/2291) | `CollectorMutability` — replaces manual mutable-collector patterns with JDK-native unmodifiable collectors |
| 8 | **Zalando** | [logbook #2385](https://github.com/zalando/logbook/pull/2385) | `AnsiPrettyPrintingSink` + `AnsiColors` — colored pretty-printing of request/response JSON for local dev, auto-detects console vs. can be forced |
| 9 | **Zalando** | [logbook #2386](https://github.com/zalando/logbook/pull/2386) | New `logbook-jdkhttpclient` module — `LogbookHttpClient` decorator adding `java.net.http.HttpClient` support (sync `send()` complete, `sendAsync()` in progress) |
| 10 | **Zalando** | [problem #557](https://github.com/zalando/problem/pull/557) | Added `toBuilder()` to the `Problem` interface for fluent problem mutation |
| 11 | **Debezium / Red Hat** | [debezium #7462](https://github.com/debezium/debezium/pull/7462) | PostgreSQL connector slow-startup fix — `TypeRegistry.java` with ORDER BY, iterative resolution loop, batch fallback |
| 12 | **NVlabs** | [sionna #1155](https://github.com/NVlabs/sionna/pull/1155) + [#1156](https://github.com/NVlabs/sionna/pull/1156) | Fixed 3GPP spec compliance bugs in NVIDIA Sionna SDK |
| 13 | **Kestra** | [kestra #19081](https://github.com/kestra-io/kestra/pull/19081) | `fix(core)`: prevent UID collisions in `IdUtils.fromParts` |
| 14 | **Kestra** | [kestra #19219](https://github.com/kestra-io/kestra/pull/19219) | `fix(core)`: preserve title and description on retry type discriminator field |

**Orgs touched:** 🇳🇱 Zalando &nbsp;·&nbsp; 🇳🇱 Adyen &nbsp;·&nbsp; 🇳🇱 Picnic &nbsp;·&nbsp; 🌍 Debezium (Red Hat) &nbsp;·&nbsp; 🌍 Kestra &nbsp;·&nbsp; 🇺🇸 NVIDIA

---

## 🚀 Projects

### [Sionna Visualizer — 6G Research Dashboard](https://github.com/Vinu2111/sionna-visualizer)
*Angular 17 · Spring Boot 3 · Python FastAPI · PostgreSQL · JWT*

The missing visual layer for NVIDIA Sionna (200,000+ downloads). A full-stack dashboard that makes 6G simulation results visual, comparable, and shareable with a Publication Pipeline, multi-simulator comparison, and Claude API integration for natural language simulation.

NVIDIA core maintainer **Merlin Nimier-David** mentioned `@Vinu2111` by name in a GitHub discussion. Accepted into the **NVIDIA AI Aerial / 6G Developer Program**.

→ [Live](https://sionna-visualizer.vercel.app) · [GitHub](https://github.com/Vinu2111/sionna-visualizer)

---

### [Picnic Store Intelligence](https://github.com/Vinu2111/picnic-store-intelligence)
*Java 21 · Spring Boot 3.2 · PostgreSQL (Supabase) · Vanilla JS · Railway + Vercel*

An architectural prototype exploring two problems I found in Picnic's Page Platform engineering blog series: **server-driven section rendering** and **per-customer section ranking**.

The backend owns the entire page layout via a rule engine. The frontend is a dumb renderer with a UI component registry. A weighted scoring algorithm silently reranks sections per customer based on purchase behaviour — `score = (frequency × 0.5) + (recency × 0.3) + (time-of-day × 0.2)`.

→ [Live](https://picnic-store-intelligence.vercel.app) · [API / Swagger](https://picnic-store-intelligence-production.up.railway.app/swagger-ui.html) · [GitHub](https://github.com/Vinu2111/picnic-store-intelligence)

---

## 🔧 Stack

| Layer | Technologies |
|---|---|
| **Languages** | Java · Python · SQL · JavaScript |
| **Frameworks** | Spring Boot 3 · Spring Security · Spring Data JPA · FastAPI · Angular 17 |
| **Databases** | MySQL · PostgreSQL |
| **Cloud & Tools** | AWS (CCP certified) · Docker · Maven · Git · Postman · IntelliJ IDEA |
| **6G / AI** | NVIDIA Sionna SDK · NVIDIA AI Aerial / 6G Developer Program |

---

## 📝 Writing

I post daily — backend engineering concepts, OSS contribution walkthroughs, and Java deep-dives.

→ [Hashnode](https://vinayak6g.hashnode.dev) &nbsp;·&nbsp; [Dev.to](https://dev.to/vinayakgote)
