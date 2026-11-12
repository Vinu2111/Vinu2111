# Vinayak Gote

**Java backend engineer · Open-source contributor**

Merged work at Zalando, Adyen and Picnic · Contributing to OpenRewrite and LINE Armeria

[LinkedIn](https://www.linkedin.com/in/vinayakgote) · [Dev.to](https://dev.to/vinu2730) · [Portfolio](https://portfolio-gules-ten-40.vercel.app/
) · [Email](mailto:vinayakgote44@gmail.com)

Java, Spring, Python, FastAPI, Angular, PostgreSQL, MySQL, AWS, Docker, Git, Maven, IntelliJ IDEA

---

## About

I'm a backend engineer at Wipro in Pune, building production REST APIs with Java 17 and Spring Boot 3 for VodafoneIdea's telecom order management system, as part of a 7-member team. I cut average response time by about 30% through MySQL index tuning and query restructuring, and traced a recurring order-dispatch timeout to an unindexed foreign key lookup.

Outside work I contribute to open-source Java projects, mostly libraries I use or admire. I start by reproducing the problem, check it isn't already reported or fixed, and then send a small, well-tested change.

- 6 merged pull requests across Zalando, Adyen and Picnic
- Member of the NVIDIA AI Aerial / 6G Developer Program, through my work on Sionna
- AWS Certified Cloud Practitioner · NVIDIA Generative AI · Spring Boot (Scaler Academy)
- B.E. Computer Engineering, Savitribai Phule Pune University (CGPA 8.56, 2nd rank in batch)
- Learning German toward a Goethe-Institut certificate

---

## Open source

### Merged (6)

| Org | Pull request | What it does |
|---|---|---|
| Zalando | [logbook #2301](https://github.com/zalando/logbook/pull/2301) | `StatusCodeBasedSink` and `LevelBasedHttpLogWriter`: status-aware log levels (2xx/3xx → TRACE, 4xx → WARN, 5xx → ERROR) |
| Zalando | [logbook #2326](https://github.com/zalando/logbook/pull/2326) | Stops the JSON formatter embedding non-JSON bodies as invalid, unquoted JSON |
| Zalando | [logbook #2327](https://github.com/zalando/logbook/pull/2327) | Guards a bean with `@ConditionalOnClass`, fixing a startup crash without spring-web |
| Zalando | [logbook #2328](https://github.com/zalando/logbook/pull/2328) | Fixes `CachingHttpResponse` dropping attributes on `withoutBody()` |
| Adyen | [adyen-java-api-library #1952](https://github.com/Adyen/adyen-java-api-library/pull/1952) | Fixes unescaped regex dots in `Service.createBaseURL` (shipped in v42.0.0) |
| Picnic | [error-prone-support #2275](https://github.com/PicnicSupermarket/error-prone-support/pull/2275) | Refaster rule: `Optional.of(x).orElse(y)` → `requireNonNull(x)` |

### In progress

| Org | Pull request | Status |
|---|---|---|
| LINE | [armeria #7120](https://github.com/line/armeria/pull/7120) | Takes TLS 1.3 into account when validating HTTP/2 cipher suites (fixes #7112). Under review |
| LINE | [armeria #7126](https://github.com/line/armeria/pull/7126) | Fixes the HTTP/2 stream reset when a service in a `serviceWorkerGroup` throws (fixes #7061). Open |
| Picnic | [error-prone-support #2291](https://github.com/PicnicSupermarket/error-prone-support/pull/2291) | `CollectorMutability` suggests JDK-native unmodifiable collectors. Under review |
| Zalando | [logbook #2386](https://github.com/zalando/logbook/pull/2386) | `logbook-jdkhttpclient` module for `java.net.http.HttpClient`. Sync `send()` done, `sendAsync()` planned |
| OpenRewrite | [rewrite-testing-frameworks #1183](https://github.com/openrewrite/rewrite-testing-frameworks/pull/1183) | `AddMissingTestAnnotation` recipe for #772. Awaiting review |
| Kestra | [kestra #19219](https://github.com/kestra-io/kestra/pull/19219) | Keeps title and description on the retry type field. Awaiting review |

### Bugs found and reproduced

| Project | Issue | What I found |
|---|---|---|
| Picnic error-prone-support | [#2336](https://github.com/PicnicSupermarket/error-prone-support/issues/2336) | `FormatStringConcatenation` copies literal `%` and `{}` fragments unescaped into rewritten format strings, causing a runtime `IllegalFormatConversionException` for AssertJ targets. Reproduced with a compiled-checker test and direct JVM execution, and confirmed not a duplicate |
| NVIDIA Sionna | [#1108](https://github.com/NVlabs/sionna/issues/1108), [#1111](https://github.com/NVlabs/sionna/issues/1111) | TR 38.901 compliance issues |

---

## Projects

**[Sionna Visualizer](https://github.com/Vinu2111/sionna-visualizer)** · Live
Angular 17, Spring Boot 3, FastAPI, PostgreSQL, JWT. A dashboard that makes NVIDIA Sionna 6G simulation results visual, comparable and shareable, with a publication pipeline, multi-simulator comparison and a Claude API integration for natural-language simulation.

**[Picnic Store Intelligence](https://github.com/Vinu2111/picnic-store-intelligence)** · Live · API docs
Java 21, Spring Boot 3.2, PostgreSQL, Vanilla JS. A prototype of two ideas from Picnic's Page Platform engineering blog series: server-driven page layouts and per-customer section ranking.

---

## Writing

I write about backend engineering, open-source contributions and Java on [Hashnode](https://hashnode.com/@vinayakgote2730) and [Dev.to](YOUR_DEVTO_URL).
