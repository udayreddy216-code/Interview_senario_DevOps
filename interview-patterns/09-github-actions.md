# 9. 🐙 GITHUB ACTIONS — 25 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🧭 Workflow Design | Trigger → Runner → Jobs → Steps → Artifacts → Status Check |
| 2 | 💥 Workflow Failure Triage | Log → Failing Step → Local Repro → Runner/Env → Fix → Rerun |
| 3 | 🔔 Trigger / Event Issues | Event Type → Filter (paths/branches) → Payload → Test Dispatch → Fix → Verify |
| 4 | 🧮 Matrix Builds | Matrix Vars → Fail-Fast → Max-Parallel → Exclude Combos → Aggregate → Optimize |
| 5 | 🧩 Custom / Composite Actions | Need → Interface (inputs/outputs) → Implementation → Test → Version Tag → Document |
| 6 | 🖥️ Self-Hosted Runner | Provision → Labels → Network/Egress → Cleanup → Autoscale → Monitor |
| 7 | 🔐 Secrets & Environments | Secret Scope → Environment Protection → Reviewers → Masking → Rotation → Audit |
| 8 | 📦 Cache / Dependency Speed | Cache Key → Restore/Save → Hit Rate → Layer Cache → Measure → Tune |
| 9 | 🔍 Debugging (logs / re-run) | Verbose Logs → Debug Logging Enabled → Re-run Failed Jobs → Artifact Download → Fix → Verify |
| 10 | 🔑 Cloud Auth (OIDC) | Provider Trust → Role/Policy → OIDC Config → No Long-Lived Keys → Test → Least Privilege |
| 11 | 🚦 Concurrency & Queueing | Concurrency Group → Cancel-In-Progress → Ordering → Runner Demand → Tune → Monitor |
| 12 | ♻️ Reusable Workflows | Common Flow → workflow_call Inputs → Secrets Pass-through → Versioning → Adopt → Maintain |
| 13 | 🛒 Marketplace Action Risk | Pin SHA → Review Source → Least Permission → Replace Risky → Scan → Policy |
| 14 | ✅ Required Status Checks | Check Name → Branch Protection → Merge Block → Bypass Audit → Fix → Enforce |
| 15 | 🏷️ Release Automation | Tag Push → Build → Changelog → Artifacts → Publish Release → Notify |
| 16 | 💰 Minutes / Cost Control | Usage Report → Runner Type → Cache → Job Splitting → Limits → Optimize |
| 17 | 🛡️ Security Scanning | CodeQL → Dependabot → Secret Scanning → Gate → Triage → Remediate |
| 18 | 🗂️ Multi-Repo / Org Automation | Shared Workflow Repo → Template → Dispatch → Version → Rollout → Govern |
| 19 | 🧪 Test Parallelization / Sharding | Split Tests → Matrix Shard → Merge Results → Coverage → Fail Fast → Optimize |
| 20 | 📤 Artifacts & Uploads | Artifact Name → Retention → Download Step → Cross-Job Pass → Cleanup → Verify |
| 21 | 🌐 Environment / Deployment Protection | Environment → Reviewers → Wait Timer → Deployment Strategy → Verify → Rollback |
| 22 | 🧯 Flaky Workflow | Failure Pattern → Retry Logic → Env Isolation → Timeout Tune → Track → Fix Root |
| 23 | 🔄 Container Build & Push | Buildx → Layer Cache → Registry Login → Multi-Arch → Scan → Push Tag |
| 24 | 📋 Workflow Governance | Repo Template → Lint (actionlint) → Review Required → Standard Steps → Docs → Enforce |
| 25 | 🤖 Automation Bots (issue/PR) | Event → Permissions (GITHUB_TOKEN) → Action Logic → Idempotency → Audit → Tune |

**Drill these:** #2 Failure, #4 Matrix, #7 Secrets, #8 Cache, #10 OIDC.
