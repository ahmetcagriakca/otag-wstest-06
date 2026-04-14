# wst06 Remote + Direct Commit + CI Required

Main'e direkt push. Ama CI green kontrolu zorunlu.

## Active Task
`math_utils.py` olustur (bkz. COMMON_TASK.md). Python ile calistir. Sonra:
- `git add math_utils.py`
- `git commit -m "add modulo_sum(a, b, m)"`
- `git push origin main`
- `.github/workflows/test.yml` tetiklenir → python run
- `gh run watch` ile CI yesil bekle

## Closure Protocol
- Commit + push main
- CI check yesil olmadan `GOREV TAMAMLANDI` YAZMA
- CI complete olunca `GOREV TAMAMLANDI`

## Rules
- Kisa cevap
- Main push direkt
- CI bekle
- `GOREV TAMAMLANDI`
