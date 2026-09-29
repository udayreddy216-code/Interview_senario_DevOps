# 23. ☕ BACKEND JAVA — PART 5: HIBERNATE / JPA — 20 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🧩 Entity Mapping Issues | Field/Column Map → Annotations → Naming Strategy → Schema Match → Test → Fix |
| 2 | 🔗 Relationship Mapping | Cardinality → Owning Side → Cascade → Orphan Removal → Fetch Strategy → Test |
| 3 | 🐌 LazyInitializationException | Access Point → Session/OpenInView → Fetch Join or DTO → Refactor → Test → Prevent |
| 4 | 🔢 N+1 Query Problem | SQL Log → Association Fetch → JOIN FETCH/Batch Size → DTO Projection → Measure → Verify |
| 5 | 🧠 Session / Persistence Context | Lifecycle → Dirty Checking → Detach/Clear → Flush Mode → Test → Tune |
| 6 | 🔀 Transaction Boundaries | Service Layer Tx → Propagation → Rollback Rules → Read-Only Tx → Test → Document |
| 7 | ⚡ Second-Level Cache | Cacheable Data → Provider (Ehcache/Redis) → Invalidation → Concurrency → Measure → Tune |
| 8 | 🔍 HQL / Criteria Queries | Requirement → Query Build → Parameters → Plan/Indexes → Test → Optimize |
| 9 | 🏗️ Schema Generation Strategy | Env → ddl-auto Choice → Migration Tool (Flyway) → Validate → Diff → Automate |
| 10 | 🧯 HibernateException / StaleObjectState | Error → Cause (version/constraint) → Retry or Merge → Fix Mapping → Test → Alert |
| 11 | 🧬 Inheritance Mapping | Hierarchy Shape → Strategy (SINGLE_TABLE/JOINED) → Discriminator → Query Cost → Test → Choose |
| 12 | ⬆️ Hibernate Version Upgrade | Release Notes → API Deprecations → Dialect/Driver → Test Suite → Canary → Verify |
| 13 | 🔗 Connection Pool Integration | DataSource → Pool Config → Timeout/Leak → Metrics → Tune → Monitor |
| 14 | 🔐 Sensitive Data / Encryption | Field List → AttributeConverter → Key Management → Query Impact → Test → Audit |
| 15 | 🐛 Debugging SQL | show_sql/format → P6Spy/Log → Bind Params → Compare with DB Plan → Fix → Verify |
| 16 | 🔄 Data Migration / Bulk Update | Volume → Batch Size → JPQL/SQL Bulk → Tx Chunk → Verify Counts → Rollback Plan |
| 17 | 🔒 Optimistic / Pessimistic Locking | Concurrency Need → @Version or Lock Mode → Retry Logic → Deadlock Risk → Test → Document |
| 18 | 📊 Performance Tuning | Baseline → Fetch/Projection → Batch Inserts → Read-Only → Cache → Measure Gain |
| 19 | 🧪 Testing Persistence | Testcontainers/H2 → Seed → Assertions → Flush/Clear → CI → Fix Flaky |
| 20 | 📋 Mapping Audit / Best Practice | DTO vs Entity → Equals/HashCode → Open Session in View → Field Access → Refactor → Enforce |

**Drill these:** #3 LazyInitialization, #4 N+1, #2 Relationships, #6 Transactions, #17 Locking.
