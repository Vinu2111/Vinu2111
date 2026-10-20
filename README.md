<h1 align="center">Vinayak Gote</h1>

<p align="center">
  Java backend engineer · Open-source contributor<br/>
  Zalando · Adyen · Picnic · OpenRewrite
</p>

<p align="center">
  <a href="https://linkedin.com/in/vinayakgote">LinkedIn</a> ·
  <a href="https://vinayak6g.hashnode.dev">Blog</a> ·
  <a href="https://dev.to/vinayakgote">Dev.to</a> ·
  <a href="https://portfolio-gules-ten-40.vercel.app">Portfolio</a> ·
  <a href="mailto:vinayakgote44@gmail.com">Email</a>
</p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,python,fastapi,angular,postgres,mysql,aws,docker,git,maven,idea" alt="Java, Spring, Python, FastAPI, Angular, PostgreSQL, MySQL, AWS, Docker, Git, Maven, IntelliJ IDEA" />
</p>

---

## About

I'm a backend engineer at Wipro in Pune, building REST APIs with Java 17 and Spring Boot 3 for an enterprise telecom order management system. Outside work I contribute to open-source Java projects, mostly libraries I use or admire.

- 6 merged pull requests across Zalando, Adyen and Picnic
- Member of the NVIDIA AI Aerial / 6G Developer Program, through my work on Sionna
- AWS Certified Cloud Practitioner
- Learning German toward a Goethe-Institut certificate

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
| Picnic | [error-prone-support #2291](https://github.com/PicnicSupermarket/error-prone-support/pull/2291) | `CollectorMutability` suggests JDK-native unmodifiable collectors. Approved, waiting on a second review |
| Zalando | [logbook #2386](https://github.com/zalando/logbook/pull/2386) | `logbook-jdkhttpclient` module for `java.net.http.HttpClient`. Sync `send()` done, `sendAsync()` planned |
| OpenRewrite | [rewrite-testing-frameworks #1183](https://github.com/openrewrite/rewrite-testing-frameworks/pull/1183) | `AddMissingTestAnnotation` recipe for [#772](https://github.com/openrewrite/rewrite-testing-frameworks/issues/772). Awaiting review |
| Kestra | [kestra #19219](https://github.com/kestra-io/kestra/pull/19219) | Keeps title and description on the retry `type` field. Awaiting review |
| Kestra | [kestra #19081](https://github.com/kestra-io/kestra/pull/19081) | Fixes UID collisions in `IdUtils.fromParts`. On hold pending a maintainer decision |

<details>
<summary>Other contributions</summary>

- Submitted fixes for TR 38.901 compliance issues in NVIDIA Sionna ([#1108](https://github.com/NVlabs/sionna/issues/1108), [#1111](https://github.com/NVlabs/sionna/issues/1111))
- Reported a `FormatStringConcatenation` bug in Picnic's error-prone-support ([#2336](https://github.com/PicnicSupermarket/error-prone-support/issues/2336))

</details>

## Projects

**[Sionna Visualizer](https://github.com/Vinu2111/sionna-visualizer)** · [Live](https://sionna-visualizer.vercel.app)
Angular 17, Spring Boot 3, FastAPI, PostgreSQL, JWT.
A dashboard that makes NVIDIA Sionna 6G simulation results visual, comparable and shareable, with a publication pipeline, multi-simulator comparison and a Claude API integration for natural-language simulation.

**[Picnic Store Intelligence](https://github.com/Vinu2111/picnic-store-intelligence)** · [Live](https://picnic-store-intelligence.vercel.app) · [API docs](https://picnic-store-intelligence-production.up.railway.app/swagger-ui.html)
Java 21, Spring Boot 3.2, PostgreSQL, Vanilla JS.
A prototype of two ideas from Picnic's Page Platform engineering blog series: server-driven page layouts and per-customer section ranking.

## Writing

I write about backend engineering, open-source contributions and Java on [Hashnode](https://vinayak6g.hashnode.dev) and [Dev.to](https://dev.to/vinayakgote).
