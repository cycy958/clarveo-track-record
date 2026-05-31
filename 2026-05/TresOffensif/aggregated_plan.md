═══════════════════════════════════════════
  PLAN D'ACTION — 2026-05 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.77
═══════════════════════════════════════════

ACHATS CE MOIS (total : 4,000€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 2,450€ | 2,000–2,880€ | DCA | 3/3 |
| ETH | ACHETER | 1,550€ | 1,200–1,920€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si contagion ≥ 40 : Suspendre toutes tranches crypto restantes (passage ELEVATED→HIGH) (3/3 runs)
🔴 Si vix ≥ 25 : Suspendre achats : régime risk-on simple invalidé (1/3 runs)
🔴 Si oil_wti ≥ 115 : Suspendre achats : confirmation choc inflation pétrole (1/3 runs)
🔴 Si stablecoin_depeg ≥ 1.0 : Suspendre achats : stress stablecoin au-delà du bruit (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.97 : Suspendre achats : corrélation extrême confirmée, double exposition réelle (1/3 runs)
🔴 — : Publication CPI US / communication Fed : si choc inflation confirmé, suspendre tranches restantes (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.97 : Geler exposition risk-on, ne pas accélérer (1/3 runs)
🔴 Si oil_wti ≥ 115 : Suspendre nouvelles tranches DCA (risque inflation/taux) (1/3 runs)
🔴 Si sopr ≤ 0.98 : Stop achats crypto (bascule on-chain en pertes réalisées) (1/3 runs)
🔴 Si btc_price_eur ≤ 60000 : Stop achats crypto (rupture support psychologique) (1/3 runs)
🔴 Si stablecoin_depeg ≥ 1.0 : Suspendre achats crypto (risque systémique) (1/3 runs)
🔴 Si rsi_smh ≥ 82 : Réviser triggers ACCEL ETF (surchauffe extrême tech) (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.90 : Maintenir interdiction d'achat ETF tant que crypto en DCA (1/3 runs)
🔴 Si vix ≥ 22 : Suspendre semaines DCA restantes, attendre normalisation (1/3 runs)
🔴 Si oil_wti ≥ 110 : Suspendre achats crypto et equity, risque inflation prioritaire (1/3 runs)
🔴 Si btc_price_eur ≤ 60000 : Stop achats crypto, attendre stabilisation et nouveau brief (1/3 runs)
🔴 Si us10y ≥ 4.75 : Stop achats restants, risque repricing duration (1/3 runs)

CASH APRÈS EXÉCUTION : 16,000€ (0.0%)
ALLOCATIONS : Crypto 20.0% | ETF Core 0.0% | ETF Thématiques 0.0%
DISPERSION DES RUNS : Run1: 4,800€ — Run2: 4,000€ — Run3: 3,200€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `TresOffensif` (user `TresOffensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 5%, reçu 0.0% — profil TresOffensif
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 20.0%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 24.0% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |
| Run2 | 20.0% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |
| Run3 | 16.0% | 0.0% | 0.0% | 0.0% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*