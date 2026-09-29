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
