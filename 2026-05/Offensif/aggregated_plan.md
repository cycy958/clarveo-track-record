═══════════════════════════════════════════
  PLAN D'ACTION — 2026-05 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.77
═══════════════════════════════════════════

ACHATS CE MOIS (total : 4,350€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 2,750€ | 2,250–3,300€ | DCA | 3/3 |
| ETH | ACHETER | 1,600€ | 750–2,200€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si contagion ≥ 40 : Suspendre tous les DCA restants — passage ELEVATED → HIGH (3/3 runs)
🔴 Si vix ≥ 25 : Geler les DCA — régime Risk-On invalidé (1/3 runs)
🔴 Si oil_wti ≥ 110 : Suspendre toute entrée — risque inflation/taux renforcé (1/3 runs)
🔴 Si btc_price_eur ≤ 60000 : Stop achats market — attendre stabilisation 48h sous niveau psychologique (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.97 : Geler DCA — corrélation au-delà du percentile 100e historique, risque concentré non couvert (1/3 runs)
🔴 Si stablecoin_depeg ≤ 0.999 : Pause systémique — signal stress flux crypto (1/3 runs)
🔴 Si stablecoin_depeg ≥ 1.0 : Stop achats crypto jusqu'à normalisation (1/3 runs)
🔴 Si oil_wti ≥ 110 : Suspendre achats : choc inflationniste confirmé (1/3 runs)
🔴 Si us10y ≥ 4.70 : Suspendre achats : repricing Fed défavorable (1/3 runs)
🔴 Si btc_price_eur ≤ 60000 : Stop DCA et réévaluation : cassure seuil psychologique (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.95 : Si corrélation reste extrême ET Nasdaq corrige, suspendre (1/3 runs)
🔴 — : Prochaine publication CPI US : si surprise inflationniste, suspendre semaines restantes (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.98 : Suspendre accélération crypto (corrélation quasi parfaite, diversification nulle) (1/3 runs)
🔴 Si oil_wti ≥ 110 : Geler achats restants (+8% au-dessus de 101.94$, risque repricing inflation/taux) (1/3 runs)
🔴 Si rsi_btc ≥ 75 : Suspendre achats crypto (surachat, invalide la thèse "pas d'euphorie") (1/3 runs)
🔴 Si funding_btc ≥ 15 : Suspendre achats crypto (bascule levier long, signal d'euphorie spéculative) (1/3 runs)
🔴 Si btc_price_eur ≥ 80000 : Suspendre achats limit semaines 2-4 (rallye non confirmé par fondamentaux) (1/3 runs)
🔴 — : Annonce Fed (Powell→Warsh, mai 2026) + CPI/Fed meeting : si US10Y > 4.7 ou DXY > 102, reporter Semaine 4 (1/3 runs)

CASH APRÈS EXÉCUTION : 15,650€ (0.0%)
ALLOCATIONS : Crypto 21.7% | ETF Core 0.0% | ETF Thématiques 0.0%
DISPERSION DES RUNS : Run1: 5,500€ — Run2: 4,500€ — Run3: 3,000€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Offensif` (user `Offensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 5%, reçu 0.0% — profil Offensif
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 21.7%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 27.5% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |
| Run2 | 22.5% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |
| Run3 | 15.0% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*