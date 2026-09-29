# 7. 🧑‍🔧 JENKINS — 25 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🧭 Pipeline Design | Trigger → Stages → Agent → Build/Test → Deploy → Notify |
| 2 | 💥 Build Failure Triage | Console Log → Failing Stage → Local Repro → Fix → Rerun → Prevent |
| 3 | 🖥️ Agent / Node Offline | Node Status → Agent Log → Network/Java → Disk/Labels → Reconnect → Monitor |
| 4 | 🔑 Credentials & Secrets | Store → Scope → Masking → Rotation → Least Access → Audit |
| 5 | 🧩 Plugin Conflict / Upgrade | Broken Feature → Plugin Deps → Snapshot Backup → Upgrade → Test → Rollback Plan |
| 6 | 🐌 Slow Builds | Stage Timing → Parallelize → Cache Deps → Agent Pool → Optimize → Measure |
| 7 | 🔔 Trigger / Webhook Not Firing | SCM Poll vs Webhook → Jenkins Log → Payload → Auth/CSRF → Fix → Test Push |
| 8 | 📦 Artifact / Publish Failure | Artifact Path → Repo Auth → Network → Versioning → Retry → Verify |
| 9 | 🧠 Jenkins Master Health | Disk → Memory/GC → Queue → Thread Dump → Restart/Cleanup → Alert |
| 10 | 🔐 Jenkins Security / RBAC | Auth Realm → Matrix Roles → Job Permissions → CSRF/CLI → Harden → Audit |
| 11 | 📚 Shared Library Reuse | Common Steps → Library Repo → Version Tag → Import → Test → Rollout |
| 12 | 🧪 Quality Gates (Sonar/JUnit) | Build → Run Analysis → Gate Condition → Fail Build → Report → Fix Loop |
| 13 | ✋ Approval / Manual Gate | input Step → Approver Role → Timeout → Audit Log → Proceed/Abort → Notify |
| 14 | 💾 Jenkins Backup / DR | Config Scope (JCasC/jobs) → Backup Job → Storage → Restore Test → Schedule → Document |
| 15 | 📊 Build Metrics & Reporting | Duration → Success Rate → Flaky Tests → Dashboard → Alert → Improve |
| 16 | 🔀 Branch / Multibranch Pipeline | Repo Scan → Branch Discovery → Jenkinsfile per Branch → Cleanup → Status → Tune |
| 17 | 🐳 Docker in Jenkins | Agent Image → Socket/DinD → Cache Layers → Cleanup → Security → Test |
| 18 | 🧯 Flaky Pipeline | Failure Pattern → Retry vs Fix → Env Isolation → Stable Test → Alert → Track |
| 19 | 🔄 Rollback Deployment | Known Good Version → Deploy Stage → Verify → Rollback Path → Automate → Test |
| 20 | 🧮 Parameterized Builds | Params → Defaults → Validation → Choice Lists → Secure Values → Docs |
| 21 | 🌐 Jenkins + Cloud Agents | Demand → Cloud Plugin → Provisioning Delay → Cost → Scale Down → Monitor |
| 22 | 📜 Jenkinsfile Groovy Errors | Error Line → Sandbox/Script Approval → Syntax → Fix → Validate → Re-run |
| 23 | 🧹 Workspace / Disk Cleanup | Disk Usage → Workspace Policy → Cleanup Step → Retention → Automate → Alert |
| 24 | 🔗 Integration Failures (Artifactory/Nexus/K8s) | Endpoint → Auth → Version/API → Network → Retry → Verify |
| 25 | 📋 Pipeline as Code Governance | Jenkinsfile in Repo → Review → Lint → Shared Lib → Standard Template → Enforce |

**Drill these:** #2 Build failure, #3 Agent offline, #6 Slow builds, #1 Master health, #7 Webhook.
