# 6. 🏗️ TERRAFORM — 25 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🧠 State Locking / Conflict | Lock Info → Who Holds → Wait/Force-Unlock → Rerun → Prevent → Document |
| 2 | ☁️ Remote State Backend | Backend Config → Init → Migrate State → Locking → Access Control → Verify |
| 3 | 🌪️ Drift Detected | Plan Diff → Real Console Check → Cause → Reapply or Import → Automate Plan → Alert |
| 4 | 🧩 Module Design / Reuse | Requirement → Interface (vars/outputs) → Version Pin → Test → Publish → Document |
| 5 | 🔌 Provider Version Issues | Constraint → Lock File → Breaking Change → Pin/Upgrade → Plan Test → Apply |
| 6 | 📋 Plan vs Apply Mismatch | Read Plan → Identify Diff → Cause (drift/random) → Refresh → Replan → Verify |
| 7 | 📥 Import Existing Resource | Identify Resource → Write Config → terraform import → Plan → Apply → Document |
| 8 | 🔀 State Refactor (mv/rm) | Rename/Move → state mv or moved block → Plan Verify → Apply → Test → Commit |
| 9 | 🔐 Secrets in State | Sensitive Scan → Remote Encrypted Backend → Access Lock → Vault/Key Ref → Rotate → Policy |
| 10 | 🐌 Slow Plan / Large State | Resource Count → Parallelism → Refresh Skip → State Split → Module Split → Measure |
| 11 | 🗂️ Workspace / Environment Layout | Env Strategy (workspace vs dirs) → Vars Files → State Isolation → CI Mapping → Test → Standardize |
| 12 | 🚀 CI/CD Pipeline for IaC | Lint → fmt/validate → plan (PR) → Approve → apply → post-verify → lock state |
| 13 | 🛡️ Policy as Code | Policy Tool (OPA/Sentinel/tfsec) → Rule Set → CI Gate → Exceptions → Enforce → Report |
| 14 | 💥 Provider API Error / Throttle | Error Message → Rate Limit/Quota → Retry/Backoff → Reduce Parallelism → Rerun → Alert |
| 15 | 💾 State Corruption / Loss | Backup State → Identify Damage → Restore → Reconcile → Replan → Prevent (versioning) |
| 16 | 🧮 Variables & Outputs | Type/Default → Validation → Sensitive Mark → Output Consumption → Refactor → Document |
| 17 | 🔎 Data Sources & External | Data Need → Source Type → Dependency Order → Cache/Refresh → Test → Optimize |
| 18 | 🔗 Resource Dependency / Cycle | Graph View → depends_on → Split Resources → Remove Cycle → Plan → Verify |
| 19 | 🧯 Destroy Gone Wrong | Scope Destroy → Target/Refresh → Dependency Order → Manual Cleanup → State Sync → Document |
| 20 | 🌍 Multi-Account / Multi-Region | Requirement → State Layout → Provider Aliases → Networking → IAM → Automate |
| 21 | ⬆️ Terraform Version Upgrade | Changelog → Deprecations → Test in Non-Prod → Lock Version → CI Verify → Rollout |
| 22 | 🧪 Testing IaC | validate → plan assert → terratest → Policy Scan → CI Gate → Fix |
| 23 | 🧾 Audit / Change History | State Versioning → Plan Archive → PR Record → Tag Releases → Log → Review |
| 24 | 💰 Cost Estimation before Apply | Plan Output → Infracost → Diff Report → Approval Gate → Optimize → Track |
| 25 | 🧩 Module Registry Governance | Naming → Versioning → Docs/Examples → CI Test → Publish → Deprecation Policy |

**Drill these:** #1 State lock, #3 Drift, #7 Import, #12 CI/CD, #9 Secrets in state.
