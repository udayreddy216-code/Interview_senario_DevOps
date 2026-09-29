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
