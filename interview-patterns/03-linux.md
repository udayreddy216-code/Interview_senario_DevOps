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
