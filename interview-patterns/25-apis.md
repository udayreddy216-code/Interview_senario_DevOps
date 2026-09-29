# 25. 🔌 APIs (REST / GRAPHQL / gRPC / SOAP / WEBHOOK / ASYNC) — 25 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🧭 REST API Design | Resources → Verbs & URIs → Status Codes → Payload → Versioning → Document |
| 2 | 🔗 GraphQL Schema & Resolvers | Client Needs → Schema/Types → Resolvers → DataLoader (N+1) → Errors → Test |
| 3 | 🕸️ GraphQL Over-Fetching / Depth Attack | Query Cost → Depth/Complexity Limit → Field Whitelist → Persisted Queries → Monitor → Enforce |
| 4 | 🏷️ API Versioning Strategy | Change Type → Scheme (URI/Header) → Compatibility → Deprecation Policy → Communicate → Sunset |
| 5 | 🔐 Authentication & Authorization | AuthN (OAuth2/OIDC/API Key) → Token Scope → AuthZ Rules → Refresh/Rotation → Test → Audit |
| 6 | 🚦 Rate Limiting / Throttling | Traffic Profile → Limit Policy → 429 + Retry-After → Client Backoff → Monitor → Tune |
| 7 | 🧯 Error Handling Contract | Error Types → Standard Body (RFC7807) → Codes → Retryability → Logs → Document |
| 8 | 📘 API Documentation | Spec (OpenAPI) → Examples → Try-It Console → Change Log → Publish → Keep in Sync |
| 9 | ⚡ API Performance | Baseline Latency → Trace → N+1/DB → Cache/Compression → Pagination → Re-measure |
| 10 | 🚪 API Gateway | Routes → Auth/Policy → Throttle/Transform → Observability → Deploy → Test |
| 11 | 🔔 Webhooks | Event → Payload & Signature → Retry/Backoff → Idempotency Key → DLQ → Monitor Delivery |
| 12 | 🧪 Contract Testing | Provider Contract → Consumer Tests → Pact/Broker → CI Gate → Version → Alert on Break |
| 13 | 📡 gRPC / Protobuf | Contract (.proto) → Codegen → Streaming Type → Deadline/Retry → Versioning → Test |
| 14 | 🔄 Backward Compatibility | Change → Additive-Only Rule → Deprecate → Notify → Sunset → Verify Consumers |
| 15 | 🔐 API Security | OWASP API Top 10 → Input Validation → Secrets → CORS/mTLS → Scan → Remediate |
| 16 | 📊 API Monitoring | Latency/Error/Traffic → Per-Endpoint SLIs → Alerts → Dashboards → Traces → Review |
| 17 | 🧩 Microservice API Patterns | Service Boundary → Sync vs Async → Service Discovery → Circuit Breaker → Retry/Timeout → Trace |
| 18 | 📨 Async / Event-Driven API | Event Schema → Broker (Kafka/SQS) → Idempotent Consumer → Ordering → DLQ → Monitor Lag |
| 19 | 📦 Pagination / Filtering / Sorting | Collection Size → Style (offset/cursor) → Limits → Filter Contract → Test → Document |
| 20 | ⏱️ Timeout / Retry Strategy | Call Chain → Timeouts per Hop → Exponential Backoff → Jitter → Idempotency → Test Failure |
| 21 | 🧯 4xx vs 5xx Triage | Reproduce → Status + Body → Logs/Trace → Client vs Server → Fix → Communicate |
| 22 | 🔀 API Migration / Sunset | Consumer Inventory → New Contract → Dual Run → Traffic Shift → Sunset → Verify |
| 23 | 💾 Caching API Responses | Cacheability → ETag/Cache-Control → CDN/Redis → Invalidation → Hit Rate → Tune |
| 24 | 🌐 CORS / Preflight Failures | Origin/Method → Server CORS Config → Gateway Duplication → Credentials → Test → Fix |
| 25 | 📋 API Governance & Standards | Style Guide → Lint (Spectral) → Review Gate → Registry/Catalog → Deprecation → Report |

**Drill these:** #1 REST design, #5 Auth, #7 Errors, #9 Performance, #11 Webhooks, #2 GraphQL.
