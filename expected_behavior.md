# Expected Behavior — wst06 (direct commit + CI required)

## Workspace Config
- path: `E:\dev\otag-workspacetests\wst06_ci_required`
- git: local + remote (origin → github.com/ahmetcagriakca/otag-wstest-06)
- work_model: direct_commit
- ci_required: **true**
- qoe: disabled

## Expected Audit Steps
01-10. Coding asamasi normalden uzun — CI bekler.

## Expected Verdict
**PASS** — reviewer push + CI green evidence gorur.

## Optimization Candidates
- `closure_mode` CI-aware mi? (ci_required + direct_commit kombinasyonu)
- GOREV TAMAMLANDI CI tamamlanmadan gelirse trigger kabul ediyor mu? (premature completion riski)
- CI fail ederse review'de HOLD verilebilir mi? (beklenir)
