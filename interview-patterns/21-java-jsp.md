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
