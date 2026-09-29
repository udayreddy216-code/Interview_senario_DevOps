# 24. 🍃 BACKEND JAVA — PART 6: SPRING BOOT — 22 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 💥 Application Fails to Start | Console/Error → Bean Creation → Config/Missing Dep → Port Conflict → Fix → Restart |
| 2 | 🧩 Auto-Configuration / Bean Issues | Expected Bean → Conditions → @ComponentScan/Profile → Exclusion → Debug (–debug) → Fix |
| 3 | 💉 Dependency Injection Failure | NoSuchBean/Circular → Qualifier/Primary → Constructor Injection → Refactor → Test → Document |
| 4 | 🌐 REST API Endpoint Issue | Mapping → Method/Consumes → Params/Body Binding → Response Code → Test (curl/Postman) → Fix |
| 5 | ⚙️ Configuration / Profiles | Property Source → Precedence → Profile Activation → Externalize (Config Server/Env) → Validate → Document |
| 6 | 🗄️ Database / JPA Integration | DataSource → Dialect/ddl-auto → Migrations → Tx Manager → Test → Monitor |
| 7 | 🔐 Spring Security / JWT | Filter Chain → AuthN (JWT/OAuth2) → AuthZ Rules → CSRF/CORS → Test → Audit |
| 8 | 🩺 Actuator / Health & Metrics | Endpoints Exposed → Health Indicators → Prometheus Metrics → Alerts → Secure → Tune |
| 9 | 🚀 Deployment (JAR/Docker/K8s) | Build → Image → Env/Secrets → Probes → Rolling Deploy → Verify → Rollback |
| 10 | ⚡ Performance Tuning | Baseline → Profiler/Tracing → DB & Cache → Async/Thread Pool → Tune → Measure |
| 11 | 🧪 Testing (MockMvc/SpringBootTest) | Slice vs Full Context → Mocks → Test Data → Assertions → Coverage → CI Gate |
| 12 | 📦 Dependency / Version Conflict | Starter BOM → Conflict Tree → Exclude/Override → Rebuild → Test → Lock |
| 13 | ⬆️ Spring Boot Upgrade | Release Notes → Deprecated Props → Starter Changes → Test → Canary → Verify |
| 14 | 🪵 Logging & Tracing | Levels/Pattern → MDC Correlation ID → Logback Config → Zipkin/OTel → Centralize → Alert |
| 15 | 🧯 Exception Handling | Exception Type → @ControllerAdvice → Error Payload → Status Code → Logs → Test |
| 16 | ✅ Validation | Bean Validation Annotations → Groups → Error Messages → Custom Validator → Test → Standardize |
| 17 | 📨 Messaging (Kafka/RabbitMQ) | Topic/Queue → Producer Config → Consumer Group → Retry/DLQ → Idempotency → Monitor Lag |
| 18 | ⏰ Scheduling / Async Jobs | @Scheduled/@Async → Pool Size → Overlap Guard → Error Handling → Metrics → Tune |
| 19 | 📁 File Upload / Storage | Multipart Limits → Storage Backend (S3/Azure) → Streaming → Validation → Errors → Test |
| 20 | 🌐 CORS / Integration Errors | Preflight → Allowed Origins/Methods → Credentials → Gateway Duplicate Config → Test → Document |
| 21 | 🔗 Microservice Communication | Contract → RestTemplate/WebClient/Feign → Timeout & Retry → Circuit Breaker → Tracing → Test |
| 22 | 🧠 High Memory / Thread Exhaustion | Heap/Thread Dump → Leak or Pool Misconfig → Cache/Limits → Fix → Load Test → Alert |

**Drill these:** #1 Startup failure, #3 DI, #7 Security, #15 Exceptions, #21 Microservice calls.
