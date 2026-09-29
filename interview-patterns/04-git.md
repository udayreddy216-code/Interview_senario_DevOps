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
