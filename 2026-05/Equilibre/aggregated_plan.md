═══════════════════════════════════════════
  PLAN D'ACTION — 2026-05(2) (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.79
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,300€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 1,400€ | 1,200–1,500€ | DCA | 3/3 |
| ETH | ACHETER | 900€ | 800–1,000€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si contagion ≥ 40 : Suspendre tous achats crypto restants : passage ELEVATED→HIGH (3/3 runs)
🔴 Si stablecoin_depeg ≥ 1.0 : Suspendre limits crypto : risque exécution prioritaire (1/3 runs)
🔴 Si rsi_btc ≥ 70 : Stopper DCA BTC/ETH restant : surachat après +17.6% sur 30j (1/3 runs)
🔴 Si sp500 ≤ -8 : Suspendre achats crypto : corrélation 0.955 = transmission directe (1/3 runs)
🔴 cpi_us_release : Suspendre limits non exécutées 48h avant/après publication CPI : pétrole +79.7%/90j = risque inflation (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.97 : Suspendre DCA crypto, interdire tout achat ETF (1/3 runs)
🔴 Si oil_wti ≥ 115 : Suspendre achats jusqu'à clarification inflation/Fed (1/3 runs)
🔴 Si btc_price_eur ≤ 60000 : Stop achats crypto, réévaluer thèse de recovery (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.2 : Suspendre DCA — signal stress liquidité dollar (1/3 runs)
🔴 Si fear_greed ≥ 75 : Suspendre DCA crypto — entrée zone Greed = mauvais timing (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.97 : Suspendre achats crypto : corrélation extrême (1/3 runs)
🔴 Si oil_wti ≥ 110 : Suspendre achats : risque réinflation/choc macro (1/3 runs)
🔴 Si vix ≥ 22 : Suspendre achats crypto, conserver cash (1/3 runs)
🔴 Si dxy ≥ 102 : Suspendre achats crypto : dollar redevenu hostile (1/3 runs)
🔴 Si fear_greed ≥ 65 : Plus d'achats crypto : sentiment trop complaisant (1/3 runs)
🔴 — : Publication CPI/PCE US : si surprise inflationniste avec us10y > 4.7, suspendre (1/3 runs)

CASH APRÈS EXÉCUTION : 17,700€ (0.0%)
ALLOCATIONS : Crypto 11.5% | ETF Core 0.0% | ETF Thématiques 0.0%
DISPERSION DES RUNS : Run1: 2,500€ — Run2: 2,400€ — Run3: 2,000€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Equilibre` (user `Equilibre`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 15%, reçu 0.0% — profil Equilibre
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 11.5%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 12.5% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |
| Run2 | 12.0% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |
| Run3 | 10.0% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*