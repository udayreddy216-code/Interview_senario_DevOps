# 20. ☕ BACKEND JAVA — PART 2: DBMS / JDBC — 20 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🔗 JDBC Connectivity Failure | URL/Driver → Network/Firewall → Credentials → DB Status → Test Connect → Fix Config |
| 2 | 🧾 PreparedStatement / Injection | Query Build → Parameter Binding → Dynamic SQL Guard → Review → Test → Standardize |
| 3 | ⚡ Connection Pool Tuning (HikariCP) | Pool Metrics → Wait Time → Size vs DB Max → Leak Detection → Tune → Monitor |
| 4 | 🔀 Transaction Management | Boundary → Isolation Level → Propagation → Commit/Rollback → Test → Document |
| 5 | 🧱 Schema Design / Normalization | Requirements → ER Model → Normal Form → Indexes/Constraints → Review → Evolve |
| 6 | 🐌 Slow SQL from App | Query → EXPLAIN → Index/Join → Rewrite → Batch → Measure |
| 7 | 🧩 ORM vs JDBC Choice | Access Pattern → Complexity → Control Need → Prototype → Benchmark → Decide |
| 8 | 🔄 Migrations (Flyway/Liquibase) | Change Set → Versioning → Test on Clone → Apply → Validate → Rollback Plan |
| 9 | 🧯 Data Consistency Issue | Detect Diff → Transaction Boundary → Concurrent Update → Repair → Add Constraint → Test |
| 10 | 🔐 DB Security from App | Least-Priv User → Encryption → Secrets Store → Audit Log → Rotate → Review |
| 11 | 💾 Backup / Recovery Handling | Policy → Snapshot/Dump → Restore Test → App Behavior on Restore → Document → Automate |
| 12 | 📊 Connection Leak | Pool Stats → Unclosed Resources → try-with-resources → Leak Threshold → Fix → Alert |
| 13 | ⚖️ Deadlock / Lock Timeout from App | DB Deadlock Log → Tx Order → Shorter Tx → Retry Logic → Fix → Monitor |
| 14 | 🔀 Sharding / Read-Write Split in App | Data Volume → Shard Key → Routing Logic → Consistency Rule → Test → Monitor Lag |
| 15 | 📦 Batch Processing | Data Volume → Batch Size → Rewrite Batch Statements → Transaction Chunk → Measure → Tune |
| 16 | 🧮 Result Set / Memory Issue | Large Query → Streaming/Fetch Size → Pagination → Projection → Test → Optimize |
| 17 | 🕒 Date/Time & Timezone Bugs | Storage Type → TZ Conversion → JDBC/Driver Setting → Test Cases → Standardize UTC → Verify |
| 18 | 🧪 DB Testing | Testcontainers → Seed Data → Assertions → Cleanup → CI Integration → Fix Flaky |
| 19 | 🚦 DB Outage Handling in App | Detect → Circuit Breaker → Fallback/Cache → Retry & Backoff → Alert → Verify Recovery |
| 20 | 📋 SQL Audit / Query Governance | Slow Query Log → Top Offenders → Index Review → Code Fix → CI Lint → Report |

**Drill these:** #1 Connectivity, #3 Pool tuning, #4 Transactions, #12 Leak, #6 Slow SQL.
