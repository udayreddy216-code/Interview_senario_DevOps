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
