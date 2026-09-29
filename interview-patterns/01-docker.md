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
