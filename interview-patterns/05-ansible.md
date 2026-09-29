# 5. 🅰️ ANSIBLE — 25 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | ♻️ Idempotency Broken | Task Review → Changed on Rerun → Module Choice → Conditional → Fix → Test Twice |
| 2 | 📋 Inventory Issues | Inventory Source → Group Vars → Host Reachability → Precedence → Validate → Automate |
| 3 | 🎭 Playbook Fails Mid-Run | Error Task → Verbosity (-vvv) → Module Args → Remote State → Fix → Rerun |
| 4 | 🔑 SSH / Connectivity Failure | Ping Module → Key/User → Port/Timeout → Bastion/Jump → Fix → Verify |
| 5 | ⬆️ Privilege Escalation (become) | Sudo Rights → become_user → NOPASSWD → Test → Least Privilege → Document |
| 6 | 🧮 Variable Precedence Confusion | List Sources → Precedence Order → Where Defined → Refactor → Debug Var → Standardize |
| 7 | 🧠 Facts Slow / Wrong | Gather Facts → Fact Cache → Custom Facts → Disable When Unused → Measure → Optimize |
| 8 | 🧩 Custom Module Development | Requirement → Interface → Python/PowerShell → Unit Test → Docs → Publish |
| 9 | 📁 Roles & Collections Structure | Requirement → Role Skeleton → Defaults/Vars → Tasks/Handlers → Galaxy Publish → Version |
| 10 | 🔐 Vault / Secrets Management | Encrypt Var → Vault Password/ID → Inject at Runtime → Rotate → CI Integration → Audit |
| 11 | 🐌 Slow Playbook | Forks → Pipelining → Strategy → Serial Batches → Measure → Optimize |
| 12 | 🔁 Handlers Not Firing | Notify Name → Flush Handlers → Order → Changed Condition → Test → Fix |
| 13 | 🧯 Error Handling / Retry | Block → Rescue → Always → Retries/Delay → Fail Message → Validate |
| 14 | 🏷️ Tags for Partial Runs | Tag Tasks → List Tags → Run Subset → Verify Coverage → CI Use → Document |
| 15 | ☁️ Dynamic Inventory (Cloud) | Plugin Config → Credentials → Group Mapping → Cache → Test List → Automate |
| 16 | 🧪 Testing / Linting | ansible-lint → Syntax Check → Molecule → Idempotence Test → CI Gate → Fix |
| 17 | 🪟 Windows / Network Devices | WinRM/SSH → Module Set → Facts → Playbook Adapt → Test → Standardize |
| 18 | 🔄 CI/CD Integration | Repo → Pipeline Job → Vault Pass → Callbacks/Logs → Artifact Report → Rollback Plan |
| 19 | 🧱 Dependency / Galaxy Issues | requirements.yml → Version Pin → Install Path → Conflict → Resolve → Lock |
| 20 | 📊 Callbacks / Reporting | Callback Plugin → Output Format → Log to File/AWX → CI Summary → Alert → Review |
| 21 | 🖥️ AWX / Tower Job Failure | Job Template → Inventory/Cred → Output Log → Resource/Timeout → Fix → Rerun |
| 22 | 🧭 Drift Detection & Remediation | Desired State → Check Mode (--check) → Diff → Remediate → Schedule → Report |
| 23 | 📦 Package / Service Config | Module → State Present → Config Template → Validate → Handler Restart → Verify |
| 24 | 🚦 Rolling Deployment with Ansible | Serial → Pre/Post Checks → Health Gate → Batch → Rollback → Verify |
| 25 | 🧹 Playbook Refactor / Reuse | Duplication Scan → Roles Extract → Vars Cleanup → Docs → Test → Standardize |

**Drill these:** #1 Idempotency, #3 Playbook fails, #6 Variable precedence, #10 Vault, #11 Slow.
