# ⚡ MASTER CHEAT SHEET — one line per stack (revise in 10 minutes)

| Stack | The 3 chains you MUST know cold |
|---|---|
| 🐳 Docker | Logs → Exit Code → Entrypoint → Config → Fix → Restart  •  Scan → Prioritize CVE → Rebase → Rebuild → Retest  •  Baseline → Stats → Profile → Root Cause → Optimize → Validate |
| ☸️ Kubernetes | Describe → Logs → Exit Code → Config → Fix → Verify  •  Endpoints → Selector → Ports → NetworkPolicy → DNS → Test  •  Describe Events → Scheduler → Resources → Taint → Fix → Validate |
| 🐧 Linux | Load → Top Process → Wait Type → Fix → Validate  •  df → du → Big Files → Rotate → Cleanup → Alert  •  Ping → Route → DNS → Firewall → Port → App |
| 🌿 Git | Identify Files → Both Sides → Resolve → Test → Commit → Notify  •  Reflog → Identify → Reset/Branch → Recover → Verify  •  Detect → Rotate → Purge History → Notify → Scan Gate |
| 🅰️ Ansible | Task Review → Changed on Rerun → Module → Conditional → Test Twice  •  Error Task → -vvv → Args → Remote State → Fix → Rerun  •  Encrypt → Vault ID → Runtime Inject → Rotate → Audit |
| 🏗️ Terraform | Lock Info → Holder → Unlock → Rerun → Prevent  •  Plan Diff → Console Check → Cause → Apply/Import → Alert  •  Lint → validate → plan(PR) → approve → apply → verify |
| 🧑‍🔧 Jenkins | Console Log → Failing Stage → Local Repro → Fix → Rerun  •  Node Status → Agent Log → Network/Java → Disk → Reconnect  •  Stage Timing → Parallelize → Cache → Optimize → Measure |
| 🟦 Azure DevOps | Logs → Failing Task → Repro → Env → Fix → Rerun  •  Stages → Approvals → Pre/Post Checks → Deploy → Rollback  •  Connection Type → Auth → Scope → Test → Rotate |
| 🐙 GitHub Actions | Log → Failing Step → Repro → Runner/Env → Fix → Rerun  •  Matrix → Fail-Fast → Max-Parallel → Aggregate → Optimize  •  Secret Scope → Environment Protection → Reviewers → Rotate |
| 📊 Monitoring | Volume → Noise → Threshold → Group → Suppress → Retune  •  SLI → SLO → Burn Rate → Alert → Review  •  Detect → Triage → War Room → Mitigate → Communicate → Postmortem |
| ☁️ Azure | NSG → Route → Agent/Boot Diag → OS FW → RDP/SSH → Validate  •  Cost Analysis → Top Spend → Right-Size → Reservations → Budgets  •  Policy → Replication → Traffic Manager → Failover Test → RTO/RPO |
| 🅰️ AWS | SG → NACL → Route → Status → Logs → Validate  •  Identity → Policies → Deny → Boundary/SCP → Simulate → Least Priv  •  Metrics → Alarms → Logs Insights → SNS Action → Tune |
| 🗄️ MySQL | Query → EXPLAIN → Index/Join → Rewrite → Test → Monitor  •  Seconds Behind → Big Tx → Network → Parallel Replication → Alert  •  Deadlock Log → Lock Order → Isolation → Retry → Validate |
| 🍃 NoSQL | Access Patterns → Denormalize → Key Design → Query Test → Document  •  Hot Key → Split/Salt → Cache → Spread → Retest → Alert  •  Symptom → Read Path → Stale Replica → Quorum → Fix → Test |
| 🎨 HTML | Audit → Semantics → ARIA → Keyboard → Contrast → Retest  •  Measure LCP/CLS/INP → Critical HTML → Defer → Optimize → Re-measure |
| 🎨 CSS | Computed Style → Specificity → Order → Override → Simplify  •  Mobile-First → Breakpoints → Fluid Units → Test Devices → Fix  •  Stacking Context → Position → Layer Map → Scale System → Test |
| 🟨 JavaScript | Reproduce → Await Chain → Error Handling → Race/Timeout → Test  •  Symptom → Heap Snapshot → Detached Nodes → Fix → Compare  •  Profile → Long Tasks → Chunk/Defer → Debounce → Re-profile |
| ⚛️ React | Reproduce → State/Effect Deps → Update in Render → Fix → Guard  •  Profiler → Slow Components → memo/useMemo → Virtualize → Re-measure  •  Endpoint → Cache Key → Loading/Error → Invalidate → Test |
| ☕ Core Java | Heap Dump → Retention → Leak vs Size → GC Log → Tune  •  Thread Dump → Lock Order → Concurrent Util → Stress Test  •  GC Logs → Pause Pattern → Collector → Heap → Measure |
| ☕ DBMS/JDBC | Pool Metrics → Wait Time → Size vs DB Max → Leak Detect → Tune  •  Boundary → Isolation → Propagation → Rollback → Test  •  URL/Driver → Network → Creds → DB Status → Test |
| ☕ JSP | Error Line → Generated Servlet → Taglib → Syntax → Redeploy  •  Expression → Scope → Null → Coercion → Fix → Test  •  Output Point → Escape → Validate → CSRF Token → Test |
| ☕ Servlets | load-on-startup → init → service → destroy → Verify  •  Shared State → Instance Vars → Stateless → Load Test  •  Session Create → ID Propagation → Timeout → Invalidate → Secure |
| ☕ Hibernate | SQL Log → Association Fetch → JOIN FETCH → DTO → Measure  •  Access Point → Session → Fetch/DTO → Refactor → Prevent  •  Concurrency Need → @Version/Lock → Retry → Deadlock Risk → Test |
| 🍃 Spring Boot | Console → Bean Creation → Config/Dep → Port → Fix → Restart  •  Exception → @ControllerAdvice → Payload → Status → Logs → Test  •  Filter Chain → JWT/OAuth2 → AuthZ → CSRF/CORS → Test |
| 🔌 APIs | Resources → Verbs → Status Codes → Payload → Versioning → Docs  •  Error Types → RFC7807 Body → Codes → Retryability → Document  •  AuthN → Scope → AuthZ → Rotation → Test → Audit |

---

## 🗣️ 5 SENTENCES THAT SAVE ANY ANSWER

1. "Let me first confirm the **scope and impact** before touching anything."
2. "I gather **evidence top-down** — logs, metrics, config, then network."
3. "My priority is **mitigate first** (rollback / scale / restart), then fix the root cause."
4. "I validate the fix using **the same metric that alerted**, not just a manual check."
5. "Finally I make it **repeatable** — runbook, alert, CI guard, or automation."

## 📌 CLOSING LINE FOR EVERY SCENARIO ANSWER
> "So the flow I follow is: **[say your 6 arrows]** — and I close the loop with prevention so it doesn't repeat."
