# 14. 🍃 DATABASES — PART 2: NoSQL (Mongo / Cassandra / Redis / DynamoDB / ES) — 30 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🧩 Data Modeling | Access Patterns → Denormalize → Key/Doc Design → Query Test → Iterate → Document |
| 2 | ⚖️ Consistency Level | Requirement → Consistency Choice → Replication Factor → Trade-off → Test → Document |
| 3 | 🧮 Partition / Shard Key Design | Data Distribution → Cardinality → Hotspot Risk → Re-key → Test Load → Monitor |
| 4 | 🔥 Hot Partition / Throttling | Detect Hot Key → Split/Salt Key → Cache → Spread Writes → Retest → Alert |
| 5 | 🔁 Replication & Node Failure | Topology → Replication Factor → Repair/Rebuild → Consistency Check → Failover → Monitor |
| 6 | 💾 TTL / Compaction / Storage Growth | TTL Policy → Compaction Strategy → Disk Usage → Cleanup → Tune → Alert |
| 7 | 🐌 Slow Query / Scan | Query Pattern → Index (Secondary/Covering) → Projection/Pagination → Rewrite → Test → Monitor |
| 8 | 🔀 Migration SQL ↔ NoSQL | Schema Map → Dual Write → Backfill → Verify Parity → Cutover → Rollback Plan |
| 9 | ⚡ Caching Layer (Redis) | Cache Pattern → TTL/Eviction → Hit Rate → Stampede Guard → Invalidate → Monitor |
| 10 | 📈 Scaling Out / Rebalancing | Capacity → Add Node/Shard → Data Movement → Traffic Shift → Verify → Monitor |
| 11 | 💾 Backup / Restore / PITR | Snapshot Policy → Cross-Region Copy → Restore Test → Consistency → RPO/RTO → Automate |
| 12 | 🔐 Eventual Consistency Bug | Symptom → Read Path → Stale Replica → Read Preference/Quorum → Fix → Test |
| 13 | 💰 Serverless / On-Demand Cost | Usage Pattern → Capacity Mode → Hot/Cold Data → TTL/Tiering → Budget → Review |
| 14 | 🔍 Search / Analytics (ES) | Index Mapping → Shards/Replicas → Query DSL → Refresh Interval → Cluster Health → Tune |
| 15 | ⏱️ Time-Series Data | Ingestion Rate → Partition by Time → Retention/Downsample → Query Pattern → Storage Tier → Monitor |
| 16 | 🧱 Index Bloat / Write Amplification | Index Count → Write Cost → Drop Unused → Compound Index → Test → Monitor |
| 17 | 🔑 Data Duplication / Sync | Source of Truth → Change Streams/CDC → Idempotent Apply → Conflict Rule → Verify → Alert |
| 18 | 🧯 Cluster Unhealthy (Red/Yellow) | Health API → Unassigned Shards/Nodes → Disk Watermark → Reallocate → Recover → Prevent |
| 19 | 🔒 Security & Access | AuthN → AuthZ/Roles → Encryption (at rest/transit) → Network Isolation → Audit → Rotate |
| 20 | 🧪 Load / Performance Test | Workload Model → Baseline → Throughput/Latency → Bottleneck → Tune → Report |
| 21 | 🗑️ Large Delete / Reindex | Batch Strategy → Throttle → Reindex Task → Verify Count → Cleanup → Monitor |
| 22 | 🌐 Multi-Region / Global Tables | Conflict Resolution → Replication Lag → Local Reads → Failover → Test → Monitor |
| 23 | 📦 Document/Row Size Limits | Payload Check → Split/Limit Fields → Compression → Projection → Validate → Guard |
| 24 | 🔀 Transaction Support Limits | Need → Single-Doc vs Multi-Doc Tx → Isolation → Retry → Design Around → Document |
| 25 | 🧾 Schema Drift / Versioning | Version Field → Validator → Migration Script → Backward Compat → Test → Enforce |
| 26 | 🚦 Throughput / Rate Limit Exceeded | Provisioned vs Consumed → Retry/Backoff → Queue Writes → Autoscale Capacity → Alert → Tune |
| 27 | 🧠 Connection Pool / Driver Issue | Pool Size → Timeout → Driver Version → Retries → Monitor → Tune |
| 28 | 🔎 Aggregation Pipeline Slow | Stage Order → $match/$project Early → Index Use → explain() → Rewrite → Test |
| 29 | 💽 Disk / Memory Pressure | Metrics → Cache vs Data → Eviction → Add Storage/Node → Tune → Alert |
| 30 | 📋 NoSQL Selection Decision | Data Shape → Query Pattern → Consistency → Scale → Cost → PoC & Choose |

**Drill these:** #1 Modeling, #4 Hot partition, #9 Redis caching, #12 Eventual consistency, #8 Migration.
