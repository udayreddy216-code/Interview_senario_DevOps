# 19. ☕ BACKEND JAVA — PART 1: CORE JAVA — 20 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 💥 OutOfMemoryError | Heap Dump → Object Retention → Leak vs Size → GC Log → Fix/Tune → Validate |
| 2 | 🧠 Memory Leak Detection | Symptom → Profiler/Heap Diff → Suspect Class → Fix Reference → Retest → Monitor |
| 3 | 🗑️ GC Tuning / Long Pauses | GC Logs → Pause Pattern → Collector Choice → Heap Size → Tune → Measure |
| 4 | 🧵 Exception Handling Design | Exception Type → Catch Boundary → Custom Exception → Log & Rethrow → User Message → Test |
| 5 | 🔀 Multithreading / Deadlock | Thread Dump → Lock Order → Synchronized Scope → Concurrent Util → Fix → Stress Test |
| 6 | ⚡ Race Condition | Symptom → Shared State → Atomic/Lock → Visibility (volatile) → Test → Review |
| 7 | 🧮 Collections Performance | Access Pattern → Correct Collection → Complexity → Capacity/Load Factor → Benchmark → Optimize |
| 8 | ⚙️ JVM Tuning | Baseline → Heap/Metaspace → Flags → GC Choice → Profile → Measure Gain |
| 9 | 📁 I/O & Streams | Operation → Blocking vs NIO → Buffering → Resource Close (try-with-resources) → Test → Optimize |
| 10 | 🔤 String / Encoding Issues | Garbled Output → Charset Detect → UTF-8 Everywhere → StringBuilder for Loops → Test → Standardize |
| 11 | 🏗️ OOP / Design Refactor | Code Smell → Principle (SOLID) → Pattern Choice → Refactor → Test → Review |
| 12 | 🐛 Debugging Java App | Reproduce → Logs → Remote Debug → Breakpoint/Watch → Fix → Regression Test |
| 13 | 📦 Build / Dependency Conflict (Maven/Gradle) | Error → Dependency Tree → Version Conflict → Exclude/BOM → Rebuild → Verify |
| 14 | 🔐 Java Security | Untrusted Input → Deserialization Risk → Validation → Crypto Library → Dependency CVE → Fix |
| 15 | ⬆️ Java Version Upgrade | Release Notes → Removed APIs → Build/Test → Dep Update → Canary Deploy → Monitor |
| 16 | 🪵 Logging Strategy | Levels → Structured/JSON → MDC/Correlation → Sensitive Data Mask → Rotation → Centralize |
| 17 | 🧩 Concurrency Utils | Requirement → Executor/CompletableFuture → Timeout & Cancel → Error Handling → Test → Tune Pool |
| 18 | 🧯 High CPU in Java App | Top Threads → Thread Dump → Hot Method → Profiler → Fix/Cache → Verify |
| 19 | 📦 Serialization / JSON | Format → Library (Jackson/Gson) → Nulls & Dates → Versioning → Test → Document |
| 20 | 🧪 Testing & Mocking | Test Pyramid → JUnit/Mockito → Fixtures → Coverage → CI Gate → Fix Flaky |

**Drill these:** #1 OOM, #5 Deadlock, #3 GC, #7 Collections, #18 High CPU.
