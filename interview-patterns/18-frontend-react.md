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
