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
