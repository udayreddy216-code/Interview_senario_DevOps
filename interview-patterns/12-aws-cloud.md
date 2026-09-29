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
