# 🎯 MASTER INTERVIEW SCENARIO PATTERN BANK
### "Same way as the 20" — exhaustive case/pattern list for every tech stack

> **How to use:** Every row = one interview scenario + a 5–6 word arrow chain to memorize.
> In the interview: **name the chain out loud first**, then walk each arrow with one real example line.
> Any question, from any stack, will land on one of these chains.

---

## 📚 SECTION 0 — THE MASTER 20 (universal, stack-independent)

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🔴 Production Incident | Context → Impact → Investigate → Fix → Result → Prevention |
| 2 | 🔍 Troubleshooting | Scope → Layers → Evidence → Test → Fix → Validate |
| 3 | 🟠 Performance / Slow App | Baseline → Metrics → Bottleneck → Root Cause → Optimize → Validate |
| 4 | 🟢 Outage / Availability | Detect → Impact → Recover → Failover → Stabilize → Prevent |
| 5 | 🔵 Networking / Connectivity | DNS → Route → Security → Firewall → Port → Application |
| 6 | 🔐 Security Incident | Identity → Access → Network → Data → Monitor → Respond |
| 7 | 🚀 Deployment Failure | Plan → Validate → Deploy → Monitor → Rollback → Verify |
| 8 | ☁️ Cloud Migration | Assess → Design → Plan → Migrate → Test → Cutover |
| 9 | 📞 24/7 / On-Call | Detect → Prioritize → Troubleshoot → Communicate → Resolve → Handover |
| 10 | 👨‍💼 Behavioral | Situation → Task → Action → Result → Learning |
| 11 | 🤝 Multiple Teams | Impact → Ownership → Divide → Communicate → Update |
| 12 | 🤖 Automation | Manual → Impact → Solution → Automate → Result |
| 13 | 💰 Cost Optimization | Monitor → Identify → Analyze → Optimize → Monitor |
| 14 | 💾 Backup / DR | RPO → RTO → Backup → Replication → Failover → Test |
| 15 | 📊 Monitoring / Alerts | Metrics → Baseline → Alert → Correlate → Respond |
| 16 | 🗄️ Database Problem | Health → Performance → Queries → Connections → Backup → Recovery |
| 17 | 🔄 Change Management | Plan → Risk → Approval → Execute → Validate → Rollback |
| 18 | ⚖️ Capacity / Scaling | Demand → Metrics → Bottleneck → Scale → Validate → Monitor |
| 19 | 🛡️ High Availability | Requirements → Redundancy → Load Balance → Failover → Test → Monitor |
| 20 | 📋 Root Cause Analysis | Timeline → Evidence → Root Cause → Fix → Impact → Prevention |

---

## 🧭 THE UNIVERSAL 6-STEP ANSWER SHELL (works if you blank out)

**C → I → D → A → R → P**

| Step | Say this |
|------|----------|
| **C** Context | "First I confirm scope — what changed, since when, how many users." |
| **I** Impact | "Then I rate severity — P1/P2, business impact, and start the clock." |
| **D** Diagnose | "I collect evidence top-down: logs → metrics → traces → config → network." |
| **A** Action | "I apply the safest fix — mitigate first (rollback/scale/restart), then root-cause fix." |
| **R** Result | "I validate with the same metric that alerted, and communicate closure." |
| **P** Prevention | "I close with automation: alert, runbook, CI guard, or design change." |

> **Golden line for every answer:** *"Mitigate first, root-cause second, automate third."*

---

## 🗂️ INDEX  (files: `01-docker.md` … `25-apis.md`, plus `26-master-cheatsheet.md` and `ALL-IN-ONE-master-pattern-bank.md`)

| Section | Stack | Patterns |
|---|---|---|
| 1 | Docker | 30 |
| 2 | Kubernetes | 35 |
| 3 | Linux | 30 |
| 4 | Git | 30 |
| 5 | Ansible | 25 |
| 6 | Terraform | 25 |
| 7 | Jenkins | 25 |
| 8 | Azure DevOps | 25 |
| 9 | GitHub Actions | 25 |
| 10 | Monitoring & Alerting | 30 |
| 11 | Azure Cloud | 30 |
| 12 | AWS Cloud | 30 |
| 13 | Databases — Part 1 (MySQL / RDBMS) | 30 |
| 14 | Databases — Part 2 (NoSQL) | 30 |
| 15 | Front End — HTML | 20 |
| 16 | Front End — CSS | 20 |
| 17 | Front End — JavaScript | 20 |
| 18 | Front End — React | 20 |
| 19 | Backend Java — Core Java | 20 |
| 20 | Backend Java — DBMS/JDBC | 20 |
| 21 | Backend Java — JSP | 18 |
| 22 | Backend Java — Servlets | 18 |
| 23 | Backend Java — Hibernate | 20 |
| 24 | Backend Java — Spring Boot | 22 |
| 25 | APIs — REST / GraphQL / gRPC / Async | 25 |
| **TOTAL** | | **623** |

---

# 1. 🐳 DOCKER — 30 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🔨 Image Build Failure | Context → Error Line → Layer Cache → Fix → Rebuild → Verify |
| 2 | 🚢 Container Exits Immediately | Logs → Exit Code → Entrypoint → Config → Fix → Restart |
| 3 | 📦 Image Too Large | Inspect Layers → Identify Waste → Multi-Stage → Slim Base → Rebuild → Compare |
| 4 | 🌐 Container Networking | DNS → Network → Port Mapping → Firewall → Test → Document |
| 5 | 💾 Volume / Mount Issues | Type → Path → Permission → Ownership → Mount → Validate |
| 6 | 🔐 Secrets in Image | Scan → Identify → Remove → Inject at Runtime → Rotate → Policy |
| 7 | ⚙️ Dockerfile Best Practice | Base → Order Layers → Cache → Non-Root → Healthcheck → Scan |
| 8 | 🧹 Dangling Images / Disk Full | Analyze Usage → Prune → Retention Policy → Automate → Monitor |
| 9 | 🐌 Container Slow / High CPU | Baseline → Stats → Profile → Root Cause → Optimize → Validate |
| 10 | 🧠 OOMKilled Container | Limit → Usage → Leak Check → Tune Limit → Test → Alert |
| 11 | 🔄 Docker Compose Failures | Config Validate → Dependencies → Network → Env → Up → Verify |
| 12 | 🏗️ Multi-Stage Build | Build Stage → Copy Artifacts → Runtime Stage → Size Check → Test → Ship |
| 13 | 🖥️ Docker on Windows/WSL2 | Backend → Filesystem Perf → Line Endings → Resource Limit → Test → Document |
| 14 | ⬆️ Base Image CVE / Patch | Scan → Prioritize CVE → Rebase → Rebuild → Retest → Schedule |
| 15 | 📡 Registry Push/Pull Failure | Auth → Network → Tag → Permission → Retry → Automate Login |
| 16 | 🩺 Container Healthcheck | Define Check → Interval → Retries → Unhealthy Action → Alert → Tune |
| 17 | 🚦 Resource Limits (CPU/Mem) | Baseline → Set Limits → Test → Observe Throttle → Tune → Enforce |
| 18 | 🗝️ Env Variables / .env Chaos | List Vars → Source of Truth → Inject → Validate → Document → Secret-Separate |
| 19 | 🐛 Debug Inside Container | Reproduce → Exec Shell → Logs → Strace/Netshoot → Fix → Verify |
| 20 | 🔁 Restart Loop / CrashLoop | Logs → Exit Code → Config → Dependency Wait → Fix → Backoff Tune |
| 21 | 🧩 Layer Cache Not Working | Inspect Order → Volatile Steps → Cache Mounts → Reorder → Rebuild → Measure |
| 22 | 🌉 Bridge vs Host vs Overlay | Requirement → Network Mode → Isolation → Performance → Test → Standardize |
| 23 | 🔒 Root Container / Privilege | Scan Config → Drop Caps → Non-Root User → Read-Only FS → Retest → Policy |
| 24 | 📤 Logs Flooding Disk | Driver → Rotation → Size Limit → Centralize → Alert → Cleanup |
| 25 | 🧪 CI Image Test | Build → Unit Test in Image → Scan → Sign → Push → Deploy |
| 26 | 🔀 Docker → Kubernetes Move | Compose Review → Manifest Map → Volumes/Secrets → Probe Add → Deploy → Validate |
| 27 | 🧊 Cold Start / Pull Latency | Image Size → Registry Region → Prefetch → Lazy Load → Cache → Measure |
| 28 | 🕸️ Service Discovery in Compose | Service Name → DNS → Depends_On → Health Gate → Retry Logic → Test |
| 29 | 🧯 Docker Daemon Down | Symptom → Daemon Logs → Socket/Disk → Restart → Recover Containers → HA Plan |
| 30 | 📋 Image Governance / Tagging | Naming Standard → Immutable Tags → Scan Gate → Sign → Registry Retention → Audit |

**Top 5 Docker answers to drill:** #2 (exits), #9 (slow/OOM), #12 (multi-stage), #4 (network), #6 (secrets).

---

# 2. ☸️ KUBERNETES — 35 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 💥 Pod CrashLoopBackOff | Describe → Logs → Exit Code → Config/Dependency → Fix → Verify |
| 2 | ⏳ Pod Pending | Describe Events → Scheduler → Resources → Node Selector/Taint → Fix → Validate |
| 3 | 🔗 Service Not Reachable | Endpoints → Selector → Ports → NetworkPolicy → DNS → Test |
| 4 | 📉 OOMKilled Pod | Limits → Usage → Leak Check → Tune Requests/Limits → Test → Alert |
| 5 | 🖥️ Node NotReady | Describe Node → Kubelet Logs → Runtime → Network/Disk → Recover → Prevent |
| 6 | 🖼️ ImagePullBackOff | Image Name → Tag → Registry Auth → Pull Secret → Network → Retry |
| 7 | 💾 PVC Pending / Mount Fail | StorageClass → Provisioner → PV Binding → Node Attach → Mount → Validate |
| 8 | 🌍 Ingress Not Working | Ingress Class → Controller Logs → Backend Service → Path/Host → TLS → Test |
| 9 | 🗝️ Secret / ConfigMap Wrong | Key Name → Mount Path → Reload Strategy → Restart → Validate → GitOps Source |
| 10 | 📈 Scaling (HPA/VPA) | Metric → Target → Scale Bounds → Test Load → Observe → Tune |
| 11 | 🔄 Rolling Update / Rollback | Strategy → MaxUnavailable → Readiness → Monitor → Rollback → Verify |
| 12 | 🚧 NetworkPolicy Blocking | Policy List → Pod Labels → Ingress/Egress Rule → Test Flow → Fix → Document |
| 13 | ⬆️ Cluster Upgrade | Release Notes → Deprecation Scan → Test Cluster → Upgrade Control Plane → Nodes → Validate |
| 14 | 🔐 RBAC / Permission Denied | Identity → Role → Binding → Namespace Scope → Test with auth can-i → Least Privilege |
| 15 | 🤖 Autoscaler Not Scaling | Metric Server → Custom Metric → Threshold → Cooldown → Test Load → Tune |
| 16 | 🧠 etcd Slow / Unhealthy | Latency Metrics → DB Size → Defrag/Compact → Snapshot → Backup → Monitor |
| 17 | 🕸️ CNI / Pod-to-Pod Network | Plugin Logs → IPAM Exhaustion → Node Route → MTU → DNS → Test |
| 18 | 🚦 API Server Throttled / Slow | Latency → Priority & Fairness → Client QPS → Audit Heavy Calls → Tune → Alert |
| 19 | 🎯 Scheduling / Affinity Issue | Requirements → Labels/Taints → Affinity Rules → Topology Spread → Test → Document |
| 20 | 📊 Quota / LimitRange Exceeded | Namespace Quota → Usage → Rejection Event → Right-Size → Approve → Automate |
| 21 | 🔭 Observability Gap | Metrics → Logs → Traces → Dashboards → Alerts → Runbook |
| 22 | 🗄️ StatefulSet / Persistent Data | Identity → Volume Claim Template → Order → Backup → Failover → Test Restore |
| 23 | 📜 Certificate Expired | Expiry Check → Issuer → Renewal Job → Rotate → Verify → Auto-Renew Alert |
| 24 | 🪝 Admission Webhook Failure | Webhook Logs → FailurePolicy → Timeout → Bypass/Fix → Validate → Guard |
| 25 | 🧭 DNS Resolution Failing | CoreDNS Pods → ndots/Search → Upstream → Cache → Test → Tune |
| 26 | 💿 Node DiskPressure / Eviction | Disk Usage → Image GC → Log Rotation → Ephemeral Limits → Drain → Alert |
| 27 | ⚙️ Kubelet / Container Runtime Issue | Kubelet Logs → Runtime Socket → Cgroup/Kernel → Restart → Validate → Runbook |
| 28 | ⏰ Job / CronJob Not Running | Schedule → Concurrency Policy → BackoffLimit → Logs → Fix → Verify |
| 29 | 🔑 Kubeconfig / Cluster Access | Context → Cert Expiry → Network Path → RBAC → Rotate → Secure Access |
| 30 | 🧮 Resource Waste / Over-Provision | Request vs Usage → Right-Size → VPA Recommend → Node Pool Tune → Save → Report |
| 31 | 🧯 Namespace / Cluster Drift | Git Manifests → Live Diff → Apply → Policy Gate → Automate → Audit |
| 32 | 🚨 Evicted / Preempted Pods | Priority Class → Node Pressure → QoS Class → Spread → Reschedule → Prevent |
| 33 | 🧩 Multi-Cluster / Federation | Requirement → Traffic Split → Config Sync → Identity → Failover → Monitor |
| 34 | 🛡️ Pod Security Standards | Baseline Scan → Privileged Check → Policy Mode → Fix Manifests → Enforce → Audit |
| 35 | 📦 Helm / Kustomize Release Issue | Values Diff → Template Render → Hook Failure → Rollback → Version Pin → Test |

**Top 6 K8s answers to drill:** #1 (CrashLoop), #2 (Pending), #3 (Service), #6 (ImagePull), #5 (NotReady), #11 (Rolling/Rollback).

---

# 3. 🐧 LINUX — 30 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🔥 High CPU / Load Average | Load → Top Process → Per-Core → User/System/IO Wait → Fix → Validate |
| 2 | 🧠 High Memory / Swap Thrash | Free → Top Consumer → Cache vs Used → Swap Activity → Tune → Monitor |
| 3 | 💾 Disk Full / No Space | df → du → Big Files → Log Rotation → Cleanup → Alert |
| 4 | 🧩 Inode Exhaustion | df -i → Small File Hunt → Archive → Cleanup → Prevent → Monitor |
| 5 | 🐌 High I/O Wait | iostat → Device Latency → Process I/O → Scheduler/FS → Optimize → Validate |
| 6 | 🌐 Network Connectivity | Ping → Route → DNS → Firewall → Port → Application |
| 7 | 🧱 Firewall Blocked Traffic | Rules → Chain/Policy → Log Drops → Test Port → Allow → Persist |
| 8 | ⚙️ Service Fails to Start | Status → Journal Logs → Config Syntax → Dependency → Start → Enable |
| 9 | 🔌 Boot / Init Failure | Console/Boot Log → Failed Unit → fstab/Kernel → Recovery Mode → Fix → Verify Boot |
| 10 | 🔑 SSH Access Issue | Network → sshd Logs → Key/Perm → Config → Restart → Harden |
| 11 | 🧾 Permission Denied | Effective User → File Mode → Ownership → ACL/SELinux → Fix → Verify |
| 12 | ⏰ Cron Job Not Running | Cron Logs → Syntax/Path → Env Vars → Lock/Overlap → Fix → Alert on Failure |
| 13 | 🧟 Zombie / Orphan Process | ps State → Parent PID → Signal Handling → Kill Parent → Fix Code → Monitor |
| 14 | 📜 Log Analysis / Rotation | Locate Log → Filter/Grep → Time Correlate → Rotate/Compress → Ship → Alert |
| 15 | 💥 Kernel Panic / OOPS | Panic Trace → dmesg/Oops → Module or Hardware → Update/Blacklist → Reboot → Validate |
| 16 | 📦 Package / Dependency Broken | Repo Config → Broken Deps → Version Pin → Fix/Lock → Reinstall → Verify |
| 17 | 🛡️ SELinux / AppArmor Denial | Getenforce → AVC Denial → Audit2Allow/Profile → Test Permissive → Enforce → Document |
| 18 | ⏱️ Time Drift / NTP | timedatectl → Offset → Chrony/ntpd Source → Restart → Sync → Alert on Drift |
| 19 | 🔍 DNS Resolution Local | resolv.conf → nsswitch → dig/nslookup → Upstream → Cache → Fix |
| 20 | 👤 User / Group / Sudo Issue | id → Group Membership → sudoers Syntax → visudo Test → Fix → Audit |
| 21 | 📊 Performance Baseline (USE) | Utilization → Saturation → Errors → Per Resource → Compare Baseline → Tune |
| 22 | 🧰 File System Corruption | Unmount → fsck → Backup First → Repair → Mount → Verify Data |
| 23 | 🧲 LVM / Disk Resize | PV → VG → LV Extend → FS Resize → Verify → Document |
| 24 | 🖥️ RAID / Disk Failure | Status → Failed Slot → Replace → Rebuild → Monitor → Backup Check |
| 25 | 🔧 Sysctl / Kernel Tuning | Current Value → Bottleneck → Test Change → Persist → Rollback Plan → Monitor |
| 26 | 📡 Network Performance / Drops | Throughput → Interface Errors → Ring/Queue → MTU/TCP Tuning → Retest → Alert |
| 27 | 🧊 Process Hung / Unkillable | State (D) → Stack Trace → I/O or Lock → Wait/Reboot → Fix Root → Monitor |
| 28 | 🧪 Patching / Reboot Window | CVE List → Test Node → Patch → Reboot → Validate Services → Rollout Fleet |
| 29 | 🔐 Hardening / CIS Audit | Benchmark → Scan → Gap List → Remediate → Verify → Automate |
| 30 | 🧭 Debugging Toolbox (60-sec) | uptime → dmesg → vmstat → iostat → sar → top/netstat |

**Drill these:** #1 CPU, #2 Memory, #3 Disk, #6 Network, #8 Service, #10 SSH.

---

# 4. 🌿 GIT — 30 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 💥 Merge Conflict | Identify Files → Understand Both Sides → Resolve → Test → Commit → Notify |
| 2 | 🔀 Rebase Gone Wrong | Reflog → Abort or Reset → Rebase Clean → Force-with-Lease → Verify → Document |
| 3 | 🌱 Branch Strategy | Requirement → Model (GitFlow/Trunk) → Naming → Protection → Automation → Review |
| 4 | 🧹 Messy Commit History | Log Review → Interactive Rebase → Squash/Fixup → Rewrite Message → Push → Verify |
| 5 | 😵 Detached HEAD | Status → Identify Commit → Branch It → Merge Back → Clean → Document |
| 6 | 🗑️ Accidental Commit / Push | Locate Commit → Revert (shared) or Reset (local) → Push → Verify → Guard Hook |
| 7 | 🎒 Stash Confusion | Stash List → Show/Apply → Resolve → Drop → Recover Lost → Habit Fix |
| 8 | 🔗 Remote / Fork Out of Sync | Fetch Upstream → Compare → Merge/Rebase → Push → Verify → Automate Sync |
| 9 | 🔑 Auth / Credential Failure | Error Type → Token/SSH Key → Permission → Credential Helper → Test → Secure Store |
| 10 | 🐘 Repo Too Large / LFS | Size Analysis → Big Files → LFS Migrate → History Rewrite → Verify Clone → Policy |
| 11 | 🪝 Hooks Not Working | Hook Path → Executable Bit → Logic Test → Bypass Check → Fix → Standardize (pre-commit) |
| 12 | 🏷️ Tag / Release Issue | Tag List → Correct Commit → Annotated Tag → Push Tag → Release Notes → Automate |
| 13 | 🍒 Cherry-Pick Conflict | Pick Commit → Resolve Conflict → Test → Push → Track Origin → Document |
| 14 | 🔍 Find Bug-Introducing Commit | Reproduce → git bisect → Test Script → Identify → Fix → Verify |
| 15 | 🧩 Submodule Pain | Status → Init/Update → Pin Commit → Push Submodule → Update Parent → Document |
| 16 | 📝 PR / Code Review Blocked | Diff Size → CI Status → Reviewer Assign → Address Comments → Approve → Merge |
| 17 | 🔒 Branch Protection Bypass | Policy Check → Required Checks → Admin Override Audit → Tighten → Test → Report |
| 18 | 🕳️ Lost Work / Reset Disaster | Reflog → Identify Commit → Branch/Reset → Recover Files → Verify → Backup Habit |
| 19 | 🔠 Line Ending (CRLF) Chaos | Detect Files → .gitattributes → Renormalize → Verify Diff → Team Standard → Hook |
| 20 | 🔐 Secret Committed | Detect → Rotate Secret → Purge History → Force Push → Notify → Add Scan Gate |
| 21 | 🧱 Monorepo vs Multi-Repo | Requirement → Split/Coupling → CI Impact → Tooling → Migration → Governance |
| 22 | 🚑 Partial File / Hunk Commit | Diff Review → Add -p → Stage Hunks → Commit → Verify → Repeat |
| 23 | 🔀 Merge Strategy Choice | History Cleanliness → merge/rebase/squash → Team Rule → Configure → Test → Document |
| 24 | ⏪ Revert vs Reset | Shared? → Revert (safe) → Reset (local) → Push → Verify → Communicate |
| 25 | 🧪 CI Fails Only After Merge | Reproduce Locally → Diff Base → Env/Cache → Fix → Re-run → Add Pre-Merge Check |
| 26 | 🗂️ File Rename / Move Lost History | Rename Detect → git mv → Follow Log → Verify Blame → Commit → Document |
| 27 | 🧯 Repo Corruption | Backup First → fsck → Identify Bad Object → Recover from Clone → Verify → Prevent |
| 28 | 🚀 GitOps Flow | Commit → CI Build → Manifest Update → Argo/Flux Sync → Health Check → Rollback |
| 29 | 👥 Onboarding / Clone Slow | Shallow Clone → Partial Clone → Sparse Checkout → Measure → Document → Automate |
| 30 | 📊 Git Metrics / Hygiene Audit | Commit Frequency → PR Cycle Time → Revert Rate → Repo Size → Report → Improve |

**Drill these:** #1 Conflict, #2 Rebase, #6 Undo, #18 Reflog recovery, #20 Secret leak.

---

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

---

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

---

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

---

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

---

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

---

# 10. 📊 MONITORING & ALERTING — 30 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🚨 Alert Fatigue | Alert Volume → Noise Sources → Threshold Review → Group/Dedupe → Suppress → Retune |
| 2 | ❓ Missing Data / No Metric | Collection Path → Exporter/Agent → Scrape Config → Labels → Backfill → Alert on Absence |
| 3 | 📉 Dashboard Design | Audience → Key Questions → Golden Signals → Layout → Drill-Down → Iterate |
| 4 | 📈 Metric Instrumentation | Signal Need → Metric Type (counter/gauge/histogram) → Labels → Expose → Scrape → Validate |
| 5 | 🔭 Distributed Tracing | Trace ID → Span Coverage → Sampling → Propagation → Bottleneck Span → Alert |
| 6 | 🪵 Log Aggregation | Log Source → Format/JSON → Shipper → Index → Retention → Query & Alert |
| 7 | 🎯 SLI / SLO / Error Budget | User Journey → SLI Definition → SLO Target → Burn Rate → Alert → Review |
| 8 | 🟥 Prometheus Setup | Targets → Scrape Interval → Recording Rules → Storage/TSDB → HA → Query Test |
| 9 | 🎨 Grafana Issues | Data Source → Query → Variables → Panel Type → Refresh → Alert Link |
| 10 | ⏰ Alert Rule Tuning | Baseline → Threshold → Duration (for) → Severity → Route → Test Fire |
| 11 | 📞 On-Call / Escalation Policy | Rotation → Escalation Path → Notify Channels → Ack Timeout → Handover → Review |
| 12 | 🧯 Incident Response Flow | Detect → Triage → War Room → Mitigate → Communicate → Postmortem |
| 13 | 🔮 Capacity / Trend Forecast | Historical Trend → Growth Rate → Threshold Date → Provision Plan → Alert → Review |
| 14 | 🌐 Uptime / Synthetic Checks | Endpoint List → Regions → Frequency → Assertions → Alert → Trend Report |
| 15 | ⚡ APM / App Instrumentation | Agent Install → Transaction Map → Slow Endpoints → DB Calls → Errors → Alert |
| 16 | 🧮 Cardinality Explosion | Metric Count → Label Audit → Drop/Aggregate → Retention → Cost → Policy |
| 17 | 🔗 Alert Correlation | Timeline → Related Alerts → Dependency Map → Root Alert → Suppress Noise → Automate |
| 18 | 🧾 Audit / Compliance Monitoring | Control List → Log Source → Detection Rule → Alert → Evidence → Report |
| 19 | 🛡️ Security Monitoring (SIEM) | Telemetry → Detection Rules → Triage → Enrich → Respond → Tune |
| 20 | 💰 Monitoring Cost Control | Volume → Retention → Sampling → Tiering → Unused Dashboards → Optimize |
| 21 | 🤖 Anomaly Detection | Baseline Model → Seasonality → Deviation Score → Alert Threshold → Validate → Feedback |
| 22 | 🧭 Golden Signals / RED / USE | Choose Model → Latency/Traffic/Errors/Saturation → Instrument → Dashboard → Alert → Review |
| 23 | 🔁 Alert → Auto-Remediation | Alert → Runbook → Automation Trigger → Guard Rails → Verify → Log Action |
| 24 | 📋 Postmortem / RCA from Metrics | Timeline → Evidence → Root Cause → Fix → Impact → Prevention |
| 25 | 🧩 Custom Exporter / Integration | Metric Need → Exporter Build → Endpoint → Scrape → Dashboard → Alert |
| 26 | 🌍 Multi-Region / Multi-Cluster View | Federation → Global Labels → Unified Dashboard → Per-Region Alert → Failover Signal → Test |
| 27 | ⏱️ Time-Series Data Gaps | Gap Window → Agent/Scrape Failure → Clock Skew → Backfill → Alert → Prevent |
| 28 | 🔔 Notification Routing | Severity → Team Mapping → Channel (Pager/Slack/Email) → Quiet Hours → Escalate → Review |
| 29 | 🧪 Alert Testing / Game Day | Test Alert → Inject Fault → Verify Page → Measure MTTD/MTTR → Fix Gaps → Repeat |
| 30 | 📊 Maturity Assessment | Coverage → Quality → Actionability → Automation → Culture → Roadmap |

**Drill these:** #1 Alert fatigue, #7 SLO, #10 Tuning, #5 Tracing, #12 Incident flow.

---

# 11. ☁️ AZURE CLOUD — 30 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🖥️ VM Not Accessible | NSG → Route/Peering → Agent & Boot Diag → OS Firewall → RDP/SSH → Validate |
| 2 | 📦 VM Provisioning / Boot Failure | Quota → Image/SKU → Custom Script Logs → Disk/Network → Redeploy → Automate (IaC) |
| 3 | 🌐 App Service Issues | App Logs → Config/App Settings → Scale Plan → Networking (VNet/Private) → Deploy → Verify |
| 4 | ☸️ AKS Cluster Problems | Node Pool → kubelet/Agent → Networking (CNI) → Ingress → Upgrade → Validate |
| 5 | 💾 Storage Account / Blob | Auth (RBAC/Key/SAS) → Networking Rules → Tier/Replication → Throttling → Test → Optimize |
| 6 | 🔗 VNet / NSG / Peering | Address Space → Route Table → NSG Rules → Peering/Gateway → DNS → Test Flow |
| 7 | 🔐 Entra ID (AAD) / SSO | User/Group → App Registration → Redirect/Claims → MFA & Conditional Access → Test → Audit |
| 8 | 💰 Azure Cost Optimization | Cost Analysis → Top Spend → Right-Size → Reservations/Savings → Budgets → Review |
| 9 | 💾 Backup & Site Recovery | Policy → RPO/RTO → Recovery Vault → Replication → Test Failover → Document |
| 10 | 📊 Azure Monitor / Log Analytics | Data Source → KQL Query → Alerts → Action Group → Dashboard → Tune |
| 11 | 🗄️ Azure SQL / Cosmos DB | Connectivity → DTU/RU & Throttling → Index/Query → Failover Group → Backup → Validate |
| 12 | ⚡ Azure Functions | Trigger/Binding → Timeout & Plan → Cold Start → Logs/App Insights → Retry/DLQ → Test |
| 13 | 🐳 ACR / Container Deploy | Registry SKU → Auth/Managed Identity → Image Scan → Network Rules → Pull Test → Automate |
| 14 | 🚀 CI/CD on Azure | Pipeline → Service Connection → Environment → Deploy Strategy → Verify → Rollback |
| 15 | 🚦 Quota / Throttling (429) | Limit Check → Retry-After → Backoff/Queue → Request Increase → Redesign → Monitor |
| 16 | 🛡️ Azure Policy / Governance | Initiative → Policy Assignment → Compliance Scan → Remediate → Exemptions → Report |
| 17 | 🗝️ Key Vault / Managed Identity | Access Policy vs RBAC → Soft Delete/Purge → Identity Assignment → Secret Rotation → Audit |
| 18 | 🏢 Landing Zone / Hub-Spoke | Management Groups → Subscription Split → Hub Network → Shared Services → Guardrails → Scale |
| 19 | 🧾 Compliance / Audit | Requirement → Controls → Azure Policy/Defender → Evidence Logs → Remediation → Report |
| 20 | 🌍 Region Failover / DR | Criticality → Replication (GRS/Geo) → Traffic Manager/Front Door → Failover Test → RTO/RPO → Automate |
| 21 | ⚖️ Load Balancer / Front Door / CDN | Health Probe → Rule/Routing → TLS & Cert → Cache Policy → Traffic Test → Monitor |
| 22 | 📡 Private Link / Private Endpoint | DNS Zone → Endpoint Config → Subnet/NSG → Resolution Test → Firewall Egress → Document |
| 23 | 🧯 Resource Deletion / Recovery | Soft Delete → Activity Log → Restore/Recreate → Backup Verify → Lock Resources → Prevent |
| 24 | 🔀 Azure Migration | Assess (Migrate) → Dependency Map → Waves → Replicate/Lift → Test → Cutover |
| 25 | 📈 Autoscale & Performance | Metric → Scale Rule → Cooldown → Load Test → Cost Check → Tune |
| 26 | 🧩 Event Hub / Service Bus | Throughput Units → Partition/Queue → Peek-Lock & DLQ → Backlog → Retry → Monitor |
| 27 | 🔎 Application Insights / APM | Instrument → Dependency Map → Failed Requests → Slow Calls → Alert → Fix |
| 28 | 🧪 Non-Prod / Dev-Test Cost | Schedule Shutdown → Right-Size → Spot/Low Priority → Tagging → Auto-Cleanup → Report |
| 29 | 🚨 Azure Incident (P1) | Detect → Impact → Mitigate → Failover/Scale → Communicate → RCA & Prevent |
| 30 | 📋 Azure Architecture Review | Requirements → Well-Architected Pillars → Gaps → Prioritize → Implement → Re-review |

**Drill these:** #1 VM access, #5 Storage auth, #8 Cost, #15 Throttling, #20 DR.

---

# 12. ☁️ AWS CLOUD — 30 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🖥️ EC2 Not Reachable | Security Group → NACL → Route Table → Instance Status → SSH/RDP Logs → Validate |
| 2 | 📦 EC2 Launch / Boot Failure | Quota/Limits → AMI & Key Pair → IAM Instance Profile → UserData Logs → Storage → Relaunch |
| 3 | 🪣 S3 Access / Performance | Policy & Bucket ACL → IAM → Block Public Access → Prefix/Partition → Cache/CDN → Monitor |
| 4 | ☸️ EKS Cluster Issues | Node Group → CNI/IP Exhaustion → kube-proxy/CoreDNS → IAM (IRSA) → Upgrade → Validate |
| 5 | 🔐 IAM Permission Denied | Identity → Attached Policies → Explicit Deny → Boundary/SCP → Simulate Policy → Least Privilege |
| 6 | 🌐 VPC / Subnet / Routing | CIDR & Overlap → Route Table → IGW/NAT/GW → Peering/TGW → DNS → Test Flow |
| 7 | 💰 AWS Cost Optimization | Cost Explorer → Top Services → Right-Size → Savings Plans/RIs → Lifecycle & Budgets → Review |
| 8 | 💾 Backup & DR Strategy | RPO/RTO → Backup/Vault & Snapshots → Cross-Region Copy → Failover Runbook → Test → Automate |
| 9 | 📊 CloudWatch Monitoring | Metrics → Alarms → Dashboards → Logs Insights → SNS/Actions → Tune Thresholds |
| 10 | 🗄️ RDS Performance / Availability | Metrics → Slow SQL & Indexes → Connections → Multi-AZ Failover → Read Replica → Test |
| 11 | ⚡ Lambda Issues | Timeout & Memory → Cold Start → Concurrency/Throttle → DLQ → Logs/X-Ray → Optimize |
| 12 | 🐳 ECR / ECS / Fargate | Task Definition → Image & Auth → Service Events → Networking → Scaling → Health Check |
| 13 | 🚦 Service Quotas / Throttling | Quota Check → Retry/Backoff → Request Increase → Redesign (queue/cache) → Monitor → Alert |
| 14 | 🛡️ Well-Architected Review | Pillars → Workload Assessment → High-Risk Issues → Prioritize → Remediate → Re-review |
| 15 | 🔒 Security Posture | GuardDuty → Security Hub → Config Rules → Findings Triage → Remediate → Report |
| 16 | 🌍 Route 53 / DNS | Record Set → Health Check → Routing Policy → TTL → Propagation Test → Failover Verify |
| 17 | ⚖️ Auto Scaling | Metric → Scaling Policy → Cooldown → Instance Refresh → Load Test → Cost Tune |
| 18 | 🚀 CI/CD Pipeline | Source → Build → Test → Deploy (Blue/Green) → Approval → Rollback |
| 19 | 🌐 Multi-Region / Global DR | Criticality → Replication → Global Accelerator/Route 53 → Failover Test → RTO/RPO → Automate |
| 20 | 🧾 CloudTrail / Audit | Trail Scope → Log Integrity → Event History → Findings → Retention → Alerts |
| 21 | 🔀 AWS Migration (7 R's) | Discover → Assess → Choose Strategy → Pilot Wave → Migrate → Validate & Optimize |
| 22 | 🏢 Multi-Account / Orgs | OUs → SCPs → Control Tower → SSO/Identity Center → Shared Services → Governance |
| 23 | 📊 Athena / Redshift Analytics | Data Layout → Partitioning → Query Plan → Concurrency/WLM → Cost → Optimize |
| 24 | 📨 SQS / SNS / EventBridge | Message Flow → Visibility Timeout → DLQ & Redrive → Retry → Ordering → Monitor Backlog |
| 25 | 🚪 API Gateway | Route/Stage → Auth (IAM/Cognito/Lambda) → Throttling & Quota → Cache → Logs → Test |
| 26 | 🧠 ElastiCache / DynamoDB | Hot Key/Partition → Capacity Mode → Indexes (GSI) → TTL → Backups → Throughput Tune |
| 27 | 🧯 Accidental Deletion / Recovery | Protection (Deletion/Termination) → Snapshot/Backup → Recreate → Verify → Add Guard → Document |
| 28 | 📈 Performance Troubleshooting | Baseline → X-Ray Trace → Bottleneck Service → Optimize → Load Test → Monitor |
| 29 | 🚨 AWS P1 Incident | Detect → Impact → Mitigate → Failover/Scale → Communicate → RCA & Prevent |
| 30 | 🧩 IaC / Drift in AWS | Terraform/CFN State → Drift Detect → Plan → Apply → Policy Gate → Audit |

**Drill these:** #1 EC2 access, #5 IAM denied, #7 Cost, #10 RDS, #11 Lambda, #13 Throttling.

---

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

---

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

---

# 15. 🎨 FRONT END — PART 1: HTML — 20 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🧱 Semantic Structure | Content Type → Correct Element → Hierarchy → Landmarks → Validate → Refactor |
| 2 | ♿ Accessibility (a11y) | Audit (axe/Lighthouse) → Semantics → ARIA & Labels → Keyboard → Contrast → Retest |
| 3 | 📝 Form Issues | Input Types → Labels & Name → Validation (client+server) → Error Messages → Submit UX → Test |
| 4 | 🔍 SEO Structure | Crawl Path → Title/Meta → Heading Order → Structured Data → Sitemap → Verify in GSC |
| 5 | 🌐 Cross-Browser Rendering | Reproduce → Diff per Browser → Polyfill/Normalize → Feature Detect → Test → Document |
| 6 | ⚡ Page Load / Core Web Vitals | Measure LCP/CLS/INP → Critical HTML → Defer Scripts → Optimize Media → Cache → Re-measure |
| 7 | 📱 Responsive Markup | Viewport Meta → Fluid Structure → Media Query Hooks → Touch Targets → Test Devices → Fix |
| 8 | 🖼️ Media (img/video/audio) | Format & Size → srcset/sizes → Lazy Load → Alt/Captions → Fallback → Test |
| 9 | 📦 Build / Bundling of Templates | Template Source → Preprocessor → Bundler → Minify → Cache-Bust → Verify Output |
| 10 | 🌍 i18n / RTL Markup | lang Attribute → Text Extraction → Direction & Mirroring → Localized Assets → Test → Automate |
| 11 | 🔐 Client-Side Security | Input Source → Sanitize/Escape → CSP → No Sensitive Data in Markup → Test → Review |
| 12 | 🐛 Debugging DOM | Reproduce → Inspect Elements → Computed/Events → Isolate → Fix → Verify |
| 13 | 🧩 Reusable Components / Snippets | Pattern → Markup Contract → Slots/Props → Docs → Test → Standardize |
| 14 | 🧯 Broken Page / Blank Screen | Console Errors → Network 404 → Markup/Script Order → Fix → Reload → Add Monitoring |
| 15 | 🔗 Links & Navigation | Link Audit → Relative vs Absolute → Anchor/Focus → 404 Handling → Redirect Map → Test |
| 16 | 📄 Meta / OG / Favicon | Required Tags → OG/Twitter Cards → Favicon Set → Preview Tools → Fix → Verify Share |
| 17 | 🧾 Tables & Data Display | Data Shape → thead/tbody/scope → Caption → Responsive Strategy → A11y Check → Test |
| 18 | ⏳ Loading / Skeleton States | Perceived Speed → Skeleton/Spinner → Progressive Enhance → Error State → Test → Measure |
| 19 | 🖨️ Print / Email HTML | Target Medium → Inline Styles → Table Layout → Fallbacks → Test Client → Fix |
| 20 | 📋 HTML Validation / Lint | Run Validator → Error List → Fix Semantics → CI Lint → Review → Prevent |

**Drill these:** #2 Accessibility, #3 Forms, #6 Core Web Vitals, #7 Responsive.

---

# 16. 🎨 FRONT END — PART 2: CSS — 20 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | ⚔️ Specificity / Style Not Applying | Computed Style → Selector Specificity → Source Order → Override/Refactor → Test → Simplify |
| 2 | 📐 Layout (Flexbox/Grid) | Design Intent → Container/Items → Axis & Gap → Responsive Fallback → Test → Refactor |
| 3 | 📱 Responsive / Breakpoints | Mobile-First → Breakpoint Set → Fluid Units → Test Devices → Fix Overflow → Standardize |
| 4 | 🧱 Z-Index / Stacking Chaos | Stacking Context → Position → Layer Map → Scale System → Test → Document |
| 5 | 🌐 Browser Inconsistency | Reproduce → Vendor Prefix/Autoprefixer → Normalize → Feature Query → Test Matrix → Fix |
| 6 | ✨ Animation / Transition Jank | Animate Transform/Opacity → Layer Promote → Reduced Motion → FPS Test → Optimize → Verify |
| 7 | 🌗 Theming / Dark Mode | Design Tokens → Variables → Theme Switch → Contrast Check → Test → Persist Preference |
| 8 | 🔤 Typography / Font Loading | Font Stack → preload/swap → FOUT/FOIT → Sizing Scale → Perf Impact → Verify |
| 9 | 🐛 Debug CSS | Reproduce → DevTools Computed/Box → Isolate Rule → Toggle → Fix → Regression Test |
| 10 | 🌀 Overflow / Scroll Issues | Box Model → Contain/Clip → Scroll Container → Sticky Context → Test → Fix |
| 11 | 🏗️ Architecture (BEM/Utility) | Scale Need → Naming Convention → Layers/Order → Tooling → Lint → Document |
| 12 | ♿ Accessibility in CSS | Focus Visible → Contrast Ratio → Target Size → Motion Pref → Screen Reader Test → Fix |
| 13 | 🧯 CSS Breaking After Build | Source vs Output → Purge/Tree-Shake Config → Order/Imports → Sourcemap → Fix → Test |
| 14 | ⚡ Critical CSS / Render Blocking | Measure FCP → Inline Critical → Defer Rest → Cache → Re-measure → Automate |
| 15 | 📏 CSS Variables / Design Tokens | Token Set → Scope/Inheritance → Fallbacks → Theme Use → Lint → Document |
| 16 | 🖼️ Background / Image Optimization | Format (WebP/AVIF) → Sizing → Lazy/Preload → Sprite → Test → Monitor Weight |
| 17 | 🧩 Component Style Isolation | Scope (module/shadow) → Global Leak → Override Contract → Test → Refactor → Document |
| 18 | 📐 Grid/Flex Alignment Bugs | Align vs Justify → Item Size → Min-Width/Auto → Test → Fix → Simplify |
| 19 | 🖨️ Print Stylesheet | Print Media → Page Breaks → Hide UI → Colors → Test Print → Fix |
| 20 | 📋 CSS Lint / Governance | Stylelint Config → CI Gate → Autofix → Review → Standards → Report |

**Drill these:** #1 Specificity, #2 Layout, #3 Responsive, #4 Z-index, #7 Theming.

---

# 17. 🟨 FRONT END — PART 3: JAVASCRIPT — 20 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | ⏳ Async / Promise Bugs | Reproduce → Await Chain → Error Handling → Race/Timeout → Fix → Test |
| 2 | 🧠 Memory Leak | Symptom → Heap Snapshot → Detached Nodes/Listeners → Fix → Compare → Monitor |
| 3 | 🖱️ Event Handling Issues | Event Flow (bubble/capture) → Listener Binding → Delegation → Cleanup → Test → Optimize |
| 4 | 🐛 Debugging JS | Reproduce → Breakpoints/Console → Call Stack → Isolate → Fix → Add Test |
| 5 | ⚡ Slow UI / Long Tasks | Profile → Long Task List → Chunk/Defer → Debounce/Throttle → Re-profile → Verify |
| 6 | 🗃️ State Management Bugs | State Shape → Single Source → Update Path → Stale Closure → Fix → Test |
| 7 | 📦 Module / Bundler Issues | Import Path → ESM vs CJS → Bundler Config → Tree-Shake → Build Test → Fix |
| 8 | 🧯 Error Handling Strategy | Error Types → try/catch Boundary → Global Handlers → User Message → Log/Report → Test |
| 9 | 🔠 Type Safety | Any/Unknown Usage → Types or JSDoc → Strict Mode → Compile Errors → Refactor → CI Check |
| 10 | 🔐 Client Security | Untrusted Input → Sanitize/Escape → CSP → Storage of Tokens → Prototype Pollution → Review |
| 11 | 🌐 Browser API / Compatibility | Feature → caniuse Check → Polyfill/Fallback → Feature Detect → Test Browsers → Ship |
| 12 | 📡 Fetch / API Errors | Request → Status/Network → Retry & Timeout → Cache → Error UI → Test Mocks |
| 13 | 🧪 Testing JS | Unit Scope → Framework → Mocks/Fakes → Coverage → CI Gate → Fix Flaky |
| 14 | 🔀 Migration / Refactor | Legacy Scan → Incremental Steps → Codemod → Tests First → Ship → Verify |
| 15 | 🕒 Performance (Load & Runtime) | Baseline → Bundle Size → Code Split → Lazy Load → Re-measure → Budget Alert |
| 16 | 🧩 Web Workers / Offloading | Heavy Task → Worker Design → Message Contract → Fallback → Test → Measure Gain |
| 17 | 💾 Storage (Local/Session/IndexedDB) | Data Need → Storage Choice → Quota/Expiry → Serialization → Migration → Privacy |
| 18 | 🔁 Debounce / Throttle / Race | Trigger Rate → Choose Strategy → Cancel Token → Test Timing → Tune → Document |
| 19 | 🧾 Logging / Observability FE | Error Source → Structured Log → Sentry/RUM → Session Replay → Alert → Fix Loop |
| 20 | 📋 Code Quality Governance | ESLint/Prettier → Rules → Pre-commit Hook → CI Gate → Review → Report |

**Drill these:** #1 Async, #2 Memory leak, #5 Performance, #6 State, #8 Errors.

---

# 18. ⚛️ FRONT END — PART 4: REACT — 20 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🔁 Infinite Re-render Loop | Reproduce → State/Effect Deps → Update in Render → Fix Dependency → Test → Add Guard |
| 2 | 🗃️ State Management Design | State Type (local/shared/server) → Location → Update Flow → DevTools Trace → Refactor → Test |
| 3 | 🎣 useEffect Bugs | Effect Intent → Dependency Array → Cleanup → Race/Strict Mode → Fix → Test |
| 4 | 🔑 List Rendering / Key Issues | Data Source → Stable Key → Reorder Behavior → Memoization → Test → Fix |
| 5 | 🧠 Memory Leak in Components | Symptom → Unmounted SetState/Timer/Subscription → Cleanup → Profiler → Fix → Test |
| 6 | 📦 Code Splitting / Lazy Load | Route/Component Weight → React.lazy + Suspense → Fallback → Prefetch → Measure → Tune |
| 7 | 🧭 Routing Issues | Route Config → Params/Query → Nested & Protected → Redirect/404 → Test → Fix |
| 8 | 📝 Forms & Validation | Controlled Inputs → Schema Validation → Error Display → Submit State → Test → UX Polish |
| 9 | 🌐 Context / Prop Drilling | Data Consumers → Context Boundary → Re-render Cost → Split/Memo → Test → Refactor |
| 10 | 🧯 Error Boundary / Crash UI | Failure Point → Boundary Placement → Fallback UI → Log/Report → Retry → Test |
| 11 | 📡 Data Fetching / React Query | Endpoint → Cache Key → Loading/Error States → Refetch/Invalidation → Test → Monitor |
| 12 | 🔀 Class → Hooks Migration | Component Inventory → Logic Extraction → Custom Hooks → Tests → Ship → Verify |
| 13 | 💧 SSR / Hydration Mismatch | Reproduce → Server vs Client Render → Dynamic Values → Suppress/Refactor → Test → Verify |
| 14 | 🧪 Testing React | Render → Query by Role → User Events → Mocks → Coverage → Fix Flaky |
| 15 | ⚡ Performance / Memoization | Profiler → Slow Components → memo/useMemo/useCallback → Virtualize Lists → Re-measure → Budget |
| 16 | ♿ React Accessibility | Semantics → ARIA & Labels → Focus Management → Keyboard Nav → Test (axe) → Fix |
| 17 | 🎨 Styling Approach | Design System → Method (CSS Modules/Tailwind/SC) → Theming → Isolation → Test → Standardize |
| 18 | 🧩 Custom Hook Extraction | Duplicated Logic → Hook Contract → Deps & Cleanup → Unit Test → Document → Reuse |
| 19 | ⬆️ React / Dependency Upgrade | Changelog → Breaking Changes → Codemod → Test Suite → Canary Rollout → Verify |
| 20 | 🚀 React Build & Deploy | Bundle Analyze → Env Vars → Static/CDN → Cache Headers → CI/CD → Monitor Errors |

**Drill these:** #1 Infinite loop, #3 useEffect, #11 Data fetching, #15 Performance, #13 Hydration.

---

# 19. ☕ BACKEND JAVA — PART 1: CORE JAVA — 20 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 💥 OutOfMemoryError | Heap Dump → Object Retention → Leak vs Size → GC Log → Fix/Tune → Validate |
| 2 | 🧠 Memory Leak Detection | Symptom → Profiler/Heap Diff → Suspect Class → Fix Reference → Retest → Monitor |
| 3 | 🗑️ GC Tuning / Long Pauses | GC Logs → Pause Pattern → Collector Choice → Heap Size → Tune → Measure |
| 4 | 🧵 Exception Handling Design | Exception Type → Catch Boundary → Custom Exception → Log & Rethrow → User Message → Test |
| 5 | 🔀 Multithreading / Deadlock | Thread Dump → Lock Order → Synchronized Scope → Concurrent Util → Fix → Stress Test |
| 6 | ⚡ Race Condition | Symptom → Shared State → Atomic/Lock → Visibility (volatile) → Test → Review |
| 7 | 🧮 Collections Performance | Access Pattern → Correct Collection → Complexity → Capacity/Load Factor → Benchmark → Optimize |
| 8 | ⚙️ JVM Tuning | Baseline → Heap/Metaspace → Flags → GC Choice → Profile → Measure Gain |
| 9 | 📁 I/O & Streams | Operation → Blocking vs NIO → Buffering → Resource Close (try-with-resources) → Test → Optimize |
| 10 | 🔤 String / Encoding Issues | Garbled Output → Charset Detect → UTF-8 Everywhere → StringBuilder for Loops → Test → Standardize |
| 11 | 🏗️ OOP / Design Refactor | Code Smell → Principle (SOLID) → Pattern Choice → Refactor → Test → Review |
| 12 | 🐛 Debugging Java App | Reproduce → Logs → Remote Debug → Breakpoint/Watch → Fix → Regression Test |
| 13 | 📦 Build / Dependency Conflict (Maven/Gradle) | Error → Dependency Tree → Version Conflict → Exclude/BOM → Rebuild → Verify |
| 14 | 🔐 Java Security | Untrusted Input → Deserialization Risk → Validation → Crypto Library → Dependency CVE → Fix |
| 15 | ⬆️ Java Version Upgrade | Release Notes → Removed APIs → Build/Test → Dep Update → Canary Deploy → Monitor |
| 16 | 🪵 Logging Strategy | Levels → Structured/JSON → MDC/Correlation → Sensitive Data Mask → Rotation → Centralize |
| 17 | 🧩 Concurrency Utils | Requirement → Executor/CompletableFuture → Timeout & Cancel → Error Handling → Test → Tune Pool |
| 18 | 🧯 High CPU in Java App | Top Threads → Thread Dump → Hot Method → Profiler → Fix/Cache → Verify |
| 19 | 📦 Serialization / JSON | Format → Library (Jackson/Gson) → Nulls & Dates → Versioning → Test → Document |
| 20 | 🧪 Testing & Mocking | Test Pyramid → JUnit/Mockito → Fixtures → Coverage → CI Gate → Fix Flaky |

**Drill these:** #1 OOM, #5 Deadlock, #3 GC, #7 Collections, #18 High CPU.

---

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

---

# 21. ☕ BACKEND JAVA — PART 3: JSP — 18 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 💥 JSP Compilation Error | Error Line → Generated Servlet → Taglib/Import → Syntax Fix → Redeploy → Verify |
| 2 | 🧮 EL Expression Issues | Expression → Scope Lookup → Null Handling → Type Coercion → Fix → Test |
| 3 | 🏷️ Tag Library / Custom Tag | Requirement → TLD/Tag Class → Attributes → Body Handling → Test → Document |
| 4 | 🗝️ Session / Scope Confusion | Data Lifetime → Correct Scope (page/request/session/app) → Serialization → Timeout → Test → Fix |
| 5 | 🧩 JSTL Usage | Loop/Condition → Core/SQL/Fmt Tags → Null & Empty Check → Refactor → Test → Review |
| 6 | 🔀 Include vs Forward | Static vs Dynamic → URL/Path → Parameters → Response Commit → Test → Document |
| 7 | 🚀 Deployment / Tomcat Errors | Deploy Log → WEB-INF/web.xml → Classpath → JDK Compat → Redeploy → Verify |
| 8 | ⚡ JSP Performance | Precompile → Reduce Scriptlets → Cache Fragments → Response Size → Measure → Optimize |
| 9 | 🔐 Security (XSS / CSRF) | Output Point → Escape (c:out/fn) → Input Validation → CSRF Token → Review → Test |
| 10 | 🐛 Debugging JSP | Reproduce → Generated Java → Logs → Breakpoint in Servlet → Fix → Verify |
| 11 | 🔀 Migration JSP → Thymeleaf/React | Inventory Pages → Template Map → Incremental Move → Test Parity → Cutover → Retire |
| 12 | 🧯 Page Not Found / 404-500 | URL Mapping → web.xml/Annotation → Context Path → Error Page Config → Fix → Test |
| 13 | 📝 Form Handling | Form Fields → Request Params → Validation → Redirect-After-Post → Error Display → Test |
| 14 | 🌍 i18n / Localization | Resource Bundles → fmt:setLocale → Encoding → Missing Keys → Test → Automate |
| 15 | 🖼️ Static Resource / Path Issues | Relative vs Absolute → Context Path → Cache Headers → 404 Fix → Test → Standardize |
| 16 | 🧱 Page Layout / Templating | Common Layout → include/decorator → Reuse → Consistency → Test → Refactor |
| 17 | 📊 Logging & Error Pages | Error Type → Custom Error Page → Log Detail → User-Friendly Message → Test → Monitor |
| 18 | 📋 JSP Best Practice Audit | Scriptlet Count → MVC Separation → EL/JSTL Use → Security → Refactor → Enforce |

**Drill these:** #1 Compilation, #2 EL, #4 Scopes, #9 XSS, #11 Migration.

---

# 22. ☕ BACKEND JAVA — PART 4: SERVLETS — 18 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🔄 Servlet Lifecycle | load-on-startup → init → service → doGet/doPost → destroy → Verify |
| 2 | 🔀 Request Dispatcher (forward/include) | Target Resource → Path → Attribute Passing → Response Commit → Test → Fix |
| 3 | 🗝️ Session Management | Session Creation → ID Propagation (Cookie/URL) → Timeout → Invalidation → Test → Secure Flags |
| 4 | 🧩 Filter Chain | Order → URL Pattern → doFilter Logic → Exception Path → Test → Optimize |
| 5 | 👂 Listener Events | Event Type → Listener Impl → Registration → Side-Effect Safety → Test → Log |
| 6 | ⏳ Async Servlet | startAsync → Timeout → Background Thread → Complete/Dispatch → Test → Tune |
| 7 | ⚙️ ServletContext / Init Params | Config Source → context-param vs init-param → Access Path → Change Handling → Test → Document |
| 8 | 📤 File Upload (Multipart) | Config → Size Limits → Temp Dir → Stream to Storage → Errors → Test |
| 9 | 🧯 Error Pages & Exceptions | Exception Type → error-page Config → Log Detail → User Response → Test → Monitor |
| 10 | 🧵 Thread Safety | Shared State → Instance Variables → Synchronization/Stateless → Test Under Load → Fix → Review |
| 11 | 🚀 Deployment (web.xml / Annotations) | Mapping → Conflict Check → Container Config → Deploy Log → Verify URL → Automate |
| 12 | 🔗 Connection Pool in Servlets | DataSource Lookup (JNDI) → Init Once → Close per Request → Leak Check → Test → Tune |
| 13 | 🔐 Security (Auth / CSRF / Headers) | AuthN Method → Role Check → CSRF Token → Security Headers → Review → Test |
| 14 | ⚡ Performance Tuning | Response Size → Buffering → Caching Headers → Thread Pool → Measure → Optimize |
| 15 | 🐛 Debugging Servlets | Reproduce → Container Logs → Remote Debug → Request/Response Dump → Fix → Test |
| 16 | 🌐 HTTP Method Handling | Method → idempotency → 405 Handling → Status Codes → Test → Document |
| 17 | 🔀 Migration Servlet → Spring MVC | Inventory → Controller Mapping → Interceptor/Filter Equivalents → Test Parity → Cutover → Retire |
| 18 | 📋 Servlet Best Practice Audit | Mapping Clarity → Stateless Design → Resource Cleanup → Error Handling → Security → Refactor |

**Drill these:** #1 Lifecycle, #3 Session, #4 Filters, #10 Thread safety, #8 Uploads.

---

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

---

# 24. 🍃 BACKEND JAVA — PART 6: SPRING BOOT — 22 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 💥 Application Fails to Start | Console/Error → Bean Creation → Config/Missing Dep → Port Conflict → Fix → Restart |
| 2 | 🧩 Auto-Configuration / Bean Issues | Expected Bean → Conditions → @ComponentScan/Profile → Exclusion → Debug (–debug) → Fix |
| 3 | 💉 Dependency Injection Failure | NoSuchBean/Circular → Qualifier/Primary → Constructor Injection → Refactor → Test → Document |
| 4 | 🌐 REST API Endpoint Issue | Mapping → Method/Consumes → Params/Body Binding → Response Code → Test (curl/Postman) → Fix |
| 5 | ⚙️ Configuration / Profiles | Property Source → Precedence → Profile Activation → Externalize (Config Server/Env) → Validate → Document |
| 6 | 🗄️ Database / JPA Integration | DataSource → Dialect/ddl-auto → Migrations → Tx Manager → Test → Monitor |
| 7 | 🔐 Spring Security / JWT | Filter Chain → AuthN (JWT/OAuth2) → AuthZ Rules → CSRF/CORS → Test → Audit |
| 8 | 🩺 Actuator / Health & Metrics | Endpoints Exposed → Health Indicators → Prometheus Metrics → Alerts → Secure → Tune |
| 9 | 🚀 Deployment (JAR/Docker/K8s) | Build → Image → Env/Secrets → Probes → Rolling Deploy → Verify → Rollback |
| 10 | ⚡ Performance Tuning | Baseline → Profiler/Tracing → DB & Cache → Async/Thread Pool → Tune → Measure |
| 11 | 🧪 Testing (MockMvc/SpringBootTest) | Slice vs Full Context → Mocks → Test Data → Assertions → Coverage → CI Gate |
| 12 | 📦 Dependency / Version Conflict | Starter BOM → Conflict Tree → Exclude/Override → Rebuild → Test → Lock |
| 13 | ⬆️ Spring Boot Upgrade | Release Notes → Deprecated Props → Starter Changes → Test → Canary → Verify |
| 14 | 🪵 Logging & Tracing | Levels/Pattern → MDC Correlation ID → Logback Config → Zipkin/OTel → Centralize → Alert |
| 15 | 🧯 Exception Handling | Exception Type → @ControllerAdvice → Error Payload → Status Code → Logs → Test |
| 16 | ✅ Validation | Bean Validation Annotations → Groups → Error Messages → Custom Validator → Test → Standardize |
| 17 | 📨 Messaging (Kafka/RabbitMQ) | Topic/Queue → Producer Config → Consumer Group → Retry/DLQ → Idempotency → Monitor Lag |
| 18 | ⏰ Scheduling / Async Jobs | @Scheduled/@Async → Pool Size → Overlap Guard → Error Handling → Metrics → Tune |
| 19 | 📁 File Upload / Storage | Multipart Limits → Storage Backend (S3/Azure) → Streaming → Validation → Errors → Test |
| 20 | 🌐 CORS / Integration Errors | Preflight → Allowed Origins/Methods → Credentials → Gateway Duplicate Config → Test → Document |
| 21 | 🔗 Microservice Communication | Contract → RestTemplate/WebClient/Feign → Timeout & Retry → Circuit Breaker → Tracing → Test |
| 22 | 🧠 High Memory / Thread Exhaustion | Heap/Thread Dump → Leak or Pool Misconfig → Cache/Limits → Fix → Load Test → Alert |

**Drill these:** #1 Startup failure, #3 DI, #7 Security, #15 Exceptions, #21 Microservice calls.

---

# 25. 🔌 APIs (REST / GRAPHQL / gRPC / SOAP / WEBHOOK / ASYNC) — 25 Scenario Patterns

| # | Scenario | Template to Memorize |
|---|----------|----------------------|
| 1 | 🧭 REST API Design | Resources → Verbs & URIs → Status Codes → Payload → Versioning → Document |
| 2 | 🔗 GraphQL Schema & Resolvers | Client Needs → Schema/Types → Resolvers → DataLoader (N+1) → Errors → Test |
| 3 | 🕸️ GraphQL Over-Fetching / Depth Attack | Query Cost → Depth/Complexity Limit → Field Whitelist → Persisted Queries → Monitor → Enforce |
| 4 | 🏷️ API Versioning Strategy | Change Type → Scheme (URI/Header) → Compatibility → Deprecation Policy → Communicate → Sunset |
| 5 | 🔐 Authentication & Authorization | AuthN (OAuth2/OIDC/API Key) → Token Scope → AuthZ Rules → Refresh/Rotation → Test → Audit |
| 6 | 🚦 Rate Limiting / Throttling | Traffic Profile → Limit Policy → 429 + Retry-After → Client Backoff → Monitor → Tune |
| 7 | 🧯 Error Handling Contract | Error Types → Standard Body (RFC7807) → Codes → Retryability → Logs → Document |
| 8 | 📘 API Documentation | Spec (OpenAPI) → Examples → Try-It Console → Change Log → Publish → Keep in Sync |
| 9 | ⚡ API Performance | Baseline Latency → Trace → N+1/DB → Cache/Compression → Pagination → Re-measure |
| 10 | 🚪 API Gateway | Routes → Auth/Policy → Throttle/Transform → Observability → Deploy → Test |
| 11 | 🔔 Webhooks | Event → Payload & Signature → Retry/Backoff → Idempotency Key → DLQ → Monitor Delivery |
| 12 | 🧪 Contract Testing | Provider Contract → Consumer Tests → Pact/Broker → CI Gate → Version → Alert on Break |
| 13 | 📡 gRPC / Protobuf | Contract (.proto) → Codegen → Streaming Type → Deadline/Retry → Versioning → Test |
| 14 | 🔄 Backward Compatibility | Change → Additive-Only Rule → Deprecate → Notify → Sunset → Verify Consumers |
| 15 | 🔐 API Security | OWASP API Top 10 → Input Validation → Secrets → CORS/mTLS → Scan → Remediate |
| 16 | 📊 API Monitoring | Latency/Error/Traffic → Per-Endpoint SLIs → Alerts → Dashboards → Traces → Review |
| 17 | 🧩 Microservice API Patterns | Service Boundary → Sync vs Async → Service Discovery → Circuit Breaker → Retry/Timeout → Trace |
| 18 | 📨 Async / Event-Driven API | Event Schema → Broker (Kafka/SQS) → Idempotent Consumer → Ordering → DLQ → Monitor Lag |
| 19 | 📦 Pagination / Filtering / Sorting | Collection Size → Style (offset/cursor) → Limits → Filter Contract → Test → Document |
| 20 | ⏱️ Timeout / Retry Strategy | Call Chain → Timeouts per Hop → Exponential Backoff → Jitter → Idempotency → Test Failure |
| 21 | 🧯 4xx vs 5xx Triage | Reproduce → Status + Body → Logs/Trace → Client vs Server → Fix → Communicate |
| 22 | 🔀 API Migration / Sunset | Consumer Inventory → New Contract → Dual Run → Traffic Shift → Sunset → Verify |
| 23 | 💾 Caching API Responses | Cacheability → ETag/Cache-Control → CDN/Redis → Invalidation → Hit Rate → Tune |
| 24 | 🌐 CORS / Preflight Failures | Origin/Method → Server CORS Config → Gateway Duplication → Credentials → Test → Fix |
| 25 | 📋 API Governance & Standards | Style Guide → Lint (Spectral) → Review Gate → Registry/Catalog → Deprecation → Report |

**Drill these:** #1 REST design, #5 Auth, #7 Errors, #9 Performance, #11 Webhooks, #2 GraphQL.

---

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

---

