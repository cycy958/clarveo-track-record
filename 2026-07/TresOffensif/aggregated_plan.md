═══════════════════════════════════════════
  PLAN D'ACTION — 2026-07 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.73
═══════════════════════════════════════════

ACHATS CE MOIS (total : 3,200€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 1,100€ | 800–1,250€ | DCA | 3/3 |
| EIMI | ACHETER | 150€ | 200–250€ | DCA | 2/3 |
| ETH | ACHETER | 950€ | 750–1,200€ | DCA | 3/3 |
| SKYY | ACHETER | 300€ | 150–600€ | DCA | 3/3 |
| SWRD | ACHETER | 700€ | 400–1,000€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si contagion ≥ 40 : Suspendre tous nouveaux achats crypto et ETF thématiques (passage CALM→HIGH) (2/3 runs)
🔴 Si vix ≥ 30 : Suspendre achats ETF, réduire DCA crypto aux ordres déjà posés (1/3 runs)
🔴 Si sopr ≤ 0.98 : Suspendre BTC/ETH : marché de nouveau en pertes latentes (1/3 runs)
🔴 Si funding_btc ≥ 20 : Suspendre achats BTC : levier long trop chargé (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.60 : Suspendre achats crypto si achat ETF risk-on la même semaine (double exposition) (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre achats ETF, crypto uniquement sur limites profondes (1/3 runs)
🔴 Si funding_btc ≥ 20 : Stopper achats BTC/ETH : risque de squeeze long (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Interdire achats simultanés crypto + ETF tech/thématiques (1/3 runs)
🔴 Si btc_price_eur ≤ 52000 : Suspendre achats BTC/ETH : échec du rebond sous zone J-7/J-30 (1/3 runs)
🔴 Si funding_btc ≥ 12 : Suspendre achats crypto : rally trop dépendant du levier (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre achats ETF Core/Thématiques : retour régime stress (1/3 runs)
🔴 Si sopr ≤ 0.98 : Suspendre achats crypto : capitulation non purgée (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.5 : Suspendre achats ETF Core : double exposition risk-on, coussin décorrélation perdu (1/3 runs)
🔴 us10y : Publication CPI/emploi US : arbitrage humain avant accélération (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Stopper achats BTC, conserver ETH/SWRD si SOPR > 0.98 (1/3 runs)

CASH APRÈS EXÉCUTION : 12,156€ (0.0%)
ALLOCATIONS : Crypto 34.1% | ETF Core 7.3% | ETF Thématiques 2.8%
DISPERSION DES RUNS : Run1: 3,000€ — Run2: 3,000€ — Run3: 4,000€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `TresOffensif` (user `TresOffensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 5%, reçu 0.0% — profil TresOffensif
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 44.2%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 32.5% | 0.0% | 7.8% | 2.3% | 🔴 cash_min |
| Run2 | 33.9% | 0.0% | 6.1% | 2.6% | 🔴 cash_min |
| Run3 | 35.8% | 0.0% | 8.0% | 3.5% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*