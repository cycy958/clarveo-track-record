═══════════════════════════════════════════
  PLAN D'ACTION — 2026-05 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.81
═══════════════════════════════════════════

ACHATS CE MOIS (total : 1,650€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 450€ | 700–700€ | DCA | 2/3 |
| EIMI | ACHETER | 350€ | 1,000–1,000€ | DCA | 1/3 |
| ETH | ACHETER | 200€ | 300–300€ | DCA | 2/3 |
| SWRD | ACHETER | 650€ | 2,000–2,000€ | DCA | 1/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si contagion ≥ 40 : Suspendre tous les nouveaux achats ETF Core (2/3 runs)
🔴 Si vix ≥ 25 : Suspendre les tranches crypto restantes (1/3 runs)
🔴 Si btc_price_eur ≤ 58000 : Stop achats crypto, attendre stabilisation (1/3 runs)
🔴 Si fear_greed ≥ 75 : Stop DCA crypto, risque d'euphorie (1/3 runs)
🔴 Si rsi_btc ≥ 72 : Ne pas acheter BTC en surchauffe courte (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 70 : Interdire tout achat ETF dans le cycle courant (1/3 runs)
🔴 Si oil_wti ≥ 110 : Geler tout achat equity/tech (1/3 runs)
🔴 Si stablecoin_depeg ≥ 1.0 : Stop tous achats crypto, signal systémique (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.90 : Maintenir interdiction crypto + equity simultanée (1/3 runs)
🔴 Si oil_wti ≥ 115 : Suspendre achats equity, risque inflation/taux trop élevé (1/3 runs)
🔴 Si us10y ≥ 4.70 : Suspendre achats ETF Core, duration risk en hausse (1/3 runs)
🔴 Si rsi_SWRD ≥ 74 : Suspendre les tranches SWRD restantes (1/3 runs)
🔴 Si rsi_EIMI ≥ 72 : Suspendre les tranches EIMI restantes (1/3 runs)
🔴 Si sopr ≤ 0.98 : Suspendre DCA — capitulation on-chain qui précède corrections equity (1/3 runs)
🔴 Si stablecoin_depeg ≥ 1.0 : Suspendre tous achats — stress systémique (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Stop achats crypto : aggravation du depeg BUSD déjà à 0.57% = risque liquidité (1/3 runs)
🔴 Si rsi_btc ≥ 70 : Suspendre achats BTC/ETH : passage en surachat, le DCA perd son intérêt (1/3 runs)
🔴 Si oil_wti ≥ 115 : Suspendre toute exposition risk-on : aggravation du choc énergétique (déjà +79.7% sur 90j) (1/3 runs)
🔴 Si contagion ≥ 80 : Stop total : suspendre tous nouveaux achats (1/3 runs)

CASH APRÈS EXÉCUTION : 18,350€ (0.0%)
ALLOCATIONS : Crypto 3.3% | ETF Core 5.0% | ETF Thématiques 0.0%
DISPERSION DES RUNS : Run1: 1,000€ — Run2: 3,000€ — Run3: 1,000€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Defensif` (user `Defensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 20%, reçu 0.0% — profil Defensif
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 8.3%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 5.0% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |
| Run2 | 0.0% | 0.0% | 15.0% | 0.0% | 🔴 cash_min |
| Run3 | 5.0% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*