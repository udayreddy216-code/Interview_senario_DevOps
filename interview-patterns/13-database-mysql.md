# 13. 🗄️ DATABASES — PART 1: MySQL / RELATIONAL DB — 30 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🐌 Slow Query | Identify Query → EXPLAIN Plan → Index/Join Fix → Rewrite → Test → Monitor |
| 2 | 🔗 Connection Exhaustion | Max Connections → App Pool Size → Leaks → Timeout/Kill → Tune → Alert |
| 3 | 🔁 Replication Lag | Seconds Behind → Big Tx/Binlog → Network/Disk → Parallel Replication → Tune → Alert |
| 4 | 🔒 Deadlock Detected | Deadlock Log → Lock Order → Index/Isolation → Retry Logic → Fix Tx → Validate |
| 5 | 🧱 Lock Contention | Blocking Query → innodb_lock_waits → Long Tx → Kill/Optimize → Isolation Tune → Monitor |
| 6 | 🔀 Schema Migration / DDL | Change Plan → Online DDL Tool (gh-ost/pt-osc) → Test → Execute → Validate → Rollback Plan |
| 7 | 🧮 Missing / Wrong Index | Query Pattern → Cardinality → Index Design → EXPLAIN → Test Load → Remove Unused |
| 8 | 💾 Backup & Restore | Backup Type → Schedule → Verify Integrity → Restore Test → RPO/RTO → Automate |
| 9 | 🛡️ High Availability / Failover | Topology (MGR/Cluster) → Failover Trigger → VIP/Proxy → Data Consistency → Test → Monitor |
| 10 | 💿 Disk Full / DB Down | Disk Usage → Binlog/Temp Files → Purge/Archive → Grow Volume → Restart → Alert |
| 11 | 🧩 Partitioning Strategy | Data Volume → Access Pattern → Partition Key → Pruning Test → Maintenance → Monitor |
| 12 | ⚖️ Transaction & Isolation | ACID Need → Isolation Level → Lock Scope → Rollback Handling → Test → Document |
| 13 | ⬆️ Version Upgrade | Release Notes → Deprecations → Dump/Clone Test → Upgrade → Regression Test → Cutover |
| 14 | 🧾 Data Inconsistency / Corruption | Detect Diff → Binlog/Audit → Checksum (pt-table-checksum) → Repair → Resync Replica → Prevent |
| 15 | 🔤 Charset / Collation Issues | Detect Garbled Data → Column/Table Charset → Convert → Test App → Standardize utf8mb4 → Verify |
| 16 | 📊 Performance Tuning (Buffers) | Baseline → Buffer Pool/Cache Hit → Query Load → Tune my.cnf → Test → Monitor |
| 17 | 🔐 SQL Injection / DB Security | Input Path → Parameterized Query → Least-Priv DB Users → Audit Logs → WAF → Test |
| 18 | ⚡ Capacity Planning | Growth Rate → QPS/Storage → Bottleneck Forecast → Scale (Read Replica/Shard) → Test → Review |
| 19 | 🗑️ Archival / Purge Old Data | Retention Policy → Partition/Date Filter → Batch Delete → Archive Store → Vacuum/Optimize → Verify |
| 20 | 🔄 ETL / Data Pipeline Failure | Source Check → Job Logs → Schema Drift → Idempotent Reload → Backfill → Alert |
| 21 | 🧭 Query Plan Regression | Before/After Plan → Stats Stale → ANALYZE TABLE → Index/Query Fix → Pin Plan → Monitor |
| 22 | 📈 Read/Write Splitting | Write Master → Read Replicas → Proxy/Routing → Lag Awareness → Consistency Rule → Test |
| 23 | 🧯 DB CPU Spike | Top Queries → processlist → Plan Check → Kill/Throttle → Index/Cache Fix → Alert |
| 24 | 🔑 Auth / User Permission Issue | User@Host → Grants → Plugin (caching_sha2) → Test Login → Fix Grants → Audit |
| 25 | 🧪 Testing / Staging Data | Prod Snapshot → Masking → Subset → Restore → Refresh Job → Governance |
| 26 | 📦 Stored Procedure / Trigger Issue | Logic Review → Error Handling → Performance → Version → Test → Refactor Out |
| 27 | 🌐 Cross-Region / DR Replica | Latency → Async Replication → Failover Runbook → Consistency Check → Test → Monitor |
| 28 | 🧾 Audit & Compliance Logging | Requirement → General/Audit Log → Retention → Access Control → Report → Automate |
| 29 | 🔀 Sharding / Scaling Out | Shard Key → Hotspot Risk → Router/Proxy → Rebalancing → Consistency → Monitor |
| 30 | 💰 Cloud DB Cost Optimization | Instance Size → IOPS/Storage Tier → Reserved → Idle Envs → Right-Size → Report |

**Drill these:** #1 Slow query, #3 Replication lag, #4 Deadlock, #8 Backup, #2 Connections.
