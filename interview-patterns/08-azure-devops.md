# 8. 🟦 AZURE DEVOPS — 25 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🗂️ Project / Process Setup | Process Model → Areas & Iterations → Teams → Boards → Permissions → Governance |
| 2 | 🔀 Repo & Branch Policy | Repo Layout → Branch Policy → Required Reviewers → Build Validation → Merge → Audit |
| 3 | 🧭 YAML Pipeline Design | Trigger → Pool → Stages → Jobs/Steps → Artifacts → Conditions |
| 4 | 💥 Pipeline Failure Triage | Logs → Failing Task → Local Repro → Agent/Env → Fix → Rerun |
| 5 | 🚀 Release / Deployment Gates | Stages → Approvals → Pre/Post Checks → Deploy → Verify → Rollback |
| 6 | 📦 Artifacts & Feeds | Feed Setup → NuGet/npm/Maven → Upstream Sources → Auth → Retention → Scan |
| 7 | 📋 Boards / WIP & Flow | Workflow States → WIP Limits → Cycle Time → Blockers → Dashboard → Improve |
| 8 | 🖥️ Agent Pool Issues | Pool Type → Agent Online → Capabilities/Demands → Disk/Network → Restart → Monitor |
| 9 | 🔐 Variable Groups & Key Vault | Secret Source → VG Link → Permissions → Masking → Rotation → Audit |
| 10 | 🔌 Service Connections | Connection Type → Auth (SPN/Federated) → Scope → Test → Rotate → Least Privilege |
| 11 | 🧩 Extensions / Marketplace | Need → Install → Permissions → Version Pin → Test → Remove Unused |
| 12 | 👥 Permissions / Access Levels | Access Level → Security Group → Project/Repo Scope → Deny vs Allow → Test → Audit |
| 13 | 🧪 Test Plans & Automation | Test Suite → Automated Bind → Run Config → Results → Coverage → Report |
| 14 | 📘 Wiki / Documentation | Structure → Markdown → Versioning → Ownership → Review → Search |
| 15 | 📊 Analytics & Dashboards | Query/Metric → Widget → Delivery Insights → Refresh → Share → Act on Data |
| 16 | 🚚 Migration (TFS → ADO) | Assessment → Data/Identity Map → Import → Validate → Cutover → Post-Migration |
| 17 | ☁️ Deploy to Azure (Environments) | Environment → Resource → Deployment Strategy → Approvals → Verify → Rollback |
| 18 | ⏱️ Queue / Concurrency Limits | Demand → Parallel Jobs → Concurrency Group → Cancel-in-Progress → Scale → Monitor |
| 19 | 🔁 Multi-Stage CI/CD | Build → Test → Publish → Deploy Dev → Promote QA → Prod Gate |
| 20 | 💰 Cost / Parallel Job Limits | Usage → Paid Parallelism → Self-Hosted Option → Cache → Optimize → Report |
| 21 | 🧯 Template Reuse | Common Steps → YAML Template → Parameters → Versioning → Adopt → Maintain |
| 22 | 🔍 Traceability (Work Item ↔ Commit) | Branch from WI → Commit Link → PR → Build → Release → Audit Trail |
| 23 | 🛡️ Security Scanning in Pipeline | SAST → Dependency Scan → Secret Scan → Gate → Report → Remediate |
| 24 | 🧪 Environment Parity / Config Drift | Config Source → Per-Env Override → Validation → Diff → Fix → Automate |
| 25 | 📞 Pipeline Notifications | Events → Subscription → Teams/Email → Conditions → Noise Filter → Review |

**Drill these:** #3 YAML design, #4 Failure, #5 Gates, #10 Service connections, #8 Agents.
