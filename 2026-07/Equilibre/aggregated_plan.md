═══════════════════════════════════════════
  PLAN D'ACTION — 2026-07 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.70
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,500€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 450€ | 300–600€ | DCA | 3/3 |
| CNDX | ACHETER | 100€ | 300–300€ | DCA | 1/3 |
| DX2E | ACHETER | 100€ | 100–200€ | DCA | 2/3 |
| EIMI | ACHETER | 450€ | 300–600€ | DCA | 3/3 |
| ETH | ACHETER | 400€ | 350–400€ | DCA | 3/3 |
| SWRD | ACHETER | 800€ | 600–1,000€ | DCA | 3/3 |
| XDWS | ACHETER | 200€ | 150–300€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 us10y : FOMC 28-29/07 : si hawkish ou DXY>105, suspendre semaine 4 (2/3 runs)
🔴 Si funding_btc ≥ 15 : Suspendre achats BTC/ETH : levier long trop crowded (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre thématiques ; conserver Core si liquide (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Interdire nouvelle double exposition crypto+actions (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Stop achats BTC : cassure du rebond daily (1/3 runs)
🔴 Si dxy ≥ 105 : Suspendre crypto et Nasdaq-like : scénario dollar fort (1/3 runs)
🔴 Si stablecoin_depeg ≥ 1.0 : Suspendre tout crypto : stress crédit systémique (1/3 runs)
🔴 Si funding_btc ≥ 12 : Suspendre achats BTC/ETH : longs déjà surchargés (10.38%), au-dessus de 12 le risque de long squeeze devient prioritaire (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Stop achats crypto : cassure sous 50k€ invalide le rebond, structure weekly non confirmée (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre nouveaux achats ETF et crypto : retour net du stress risk-off (1/3 runs)
🔴 Si funding_btc ≥ 12 : Suspendre achats BTC/ETH : risque de long squeeze trop élevé (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Stop achats crypto 48h, attendre stabilisation (1/3 runs)
🔴 Si dxy ≥ 105 : Suspendre achats crypto et Nasdaq : confirmation resserrement dollar (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Ne plus acheter crypto et equity ensemble ; choisir l'exposition la plus décotée (1/3 runs)
🔴 Si vix ≥ 30 : Suspendre nouveaux achats crypto + tech (CNDX/SKYY) jusqu'à stabilisation (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Stop total crypto jusqu'au retour du peg (1/3 runs)
🔴 — : CPI US mi-juillet + FOMC 28-29/07 : si print CPI chaud ou ton hawkish confirmé, geler toutes les accélérations (1/3 runs)

CASH APRÈS EXÉCUTION : 15,253€ (0.0%)
ALLOCATIONS : Crypto 16.7% | ETF Core 10.7% | ETF Thématiques 2.6%
DISPERSION DES RUNS : Run1: 3,000€ — Run2: 2,400€ — Run3: 2,150€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Equilibre` (user `Equilibre`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 15%, reçu 0.0% — profil Equilibre
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 30.0%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 17.5% | 0.0% | 11.9% | 2.8% | 🔴 cash_min |
| Run2 | 16.6% | 0.0% | 10.1% | 2.8% | 🔴 cash_min |
| Run3 | 15.9% | 0.0% | 10.1% | 2.3% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*