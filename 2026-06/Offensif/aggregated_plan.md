═══════════════════════════════════════════
  PLAN D'ACTION — 2026-06 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.75
═══════════════════════════════════════════

ACHATS CE MOIS (total : 3,950€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 1,100€ | 1,000–1,300€ | DCA | 3/3 |
| CIBR | ACHETER | 100€ | 300–300€ | DCA | 1/3 |
| DFEN | ACHETER | 100€ | 300–300€ | DCA | 1/3 |
| EIMI | ACHETER | 300€ | 250–400€ | DCA | 3/3 |
| ETH | ACHETER | 1,300€ | 1,200–1,400€ | DCA | 3/3 |
| SKYY | ACHETER | 100€ | 300–300€ | DCA | 1/3 |
| SWRD | ACHETER | 800€ | 750–880€ | DCA | 3/3 |
| XDWH | ACHETER | 150€ | 200–300€ | DCA | 2/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si btc_price_eur ≤ 48000 : Stop achats BTC/ETH jusqu'au prochain run (2e jambe baissière confirmée) (1/3 runs)
🔴 Si vix ≥ 30 : Suspendre les achats ETF Core et Thématiques (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Stop total crypto (contagion stablecoin > bruit normal) (1/3 runs)
🔴 Si dxy ≥ 102 : Suspendre tranches non exécutées (durcissement conditions financières / risque hawkish Fed) (1/3 runs)
🔴 Si vix ≥ 28 : Suspendre thématiques, réduire ETF Core à 50% (1/3 runs)
🔴 Si btc_price_eur ≤ 48000 : Stop achats crypto jusqu'à stabilisation (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Suspendre crypto et altcoins (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Suspendre les achats BTC/ETH (cassure seuil psychologique) (1/3 runs)
🔴 Si vix ≥ 30 : Suspendre ETF Core et thématiques (zone panique macro) (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Geler les achats crypto (stress systémique stablecoins) (1/3 runs)
🔴 btc_nasdaq_corr : Réévaluer concentration : décorrélation protectrice perdue (1/3 runs)
🔴 sp500 : Prochain CPI/FOMC : si surprise hawkish, suspendre les ETF 7 jours (1/3 runs)
🔴 Si contagion ≥ 40 : Suspendre achats crypto (passage ELEVATED → HIGH) (1/3 runs)
🔴 Si contagion ≥ 60 : Suspendre tous les achats crypto et ETF risqués (1/3 runs)
🔴 Si contagion ≥ 80 : Stop total : aucun nouveau déploiement (1/3 runs)

CASH APRÈS EXÉCUTION : 12,706€ (0.0%)
ALLOCATIONS : Crypto 28.5% | ETF Core 5.7% | ETF Thématiques 2.7%
DISPERSION DES RUNS : Run1: 4,200€ — Run2: 4,000€ — Run3: 4,000€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Offensif` (user `Offensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 5%, reçu 0.0% — profil Offensif
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 36.9%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 29.5% | 0.0% | 6.0% | 2.0% | 🔴 cash_min |
| Run2 | 27.5% | 0.0% | 6.0% | 3.0% | 🔴 cash_min |
| Run3 | 28.5% | 0.0% | 5.0% | 3.0% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*