═══════════════════════════════════════════
  PLAN D'ACTION — 2026-06 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.73
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,550€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 850€ | 700–1,000€ | DCA | 3/3 |
| EIMI | ACHETER | 150€ | 500–500€ | DCA | 1/3 |
| ETH | ACHETER | 600€ | 500–800€ | DCA | 3/3 |
| SWRD | ACHETER | 750€ | 600–800€ | DCA | 3/3 |
| XDWH | ACHETER | 100€ | 150–200€ | DCA | 2/3 |
| XDWS | ACHETER | 100€ | 350–350€ | DCA | 1/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si contagion ≥ 55 : Suspendre tous achats crypto (DCA + ACCEL) — fuite DeFi trop rapide (2/3 runs)
🔴 Si vix ≥ 25 : Suspendre achats SWRD (sortie régime calme) (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Stopper achats crypto (au-dessus du bruit) (1/3 runs)
🔴 Si btc_price_eur ≤ 48000 : Suspendre DCA crypto (~-10% sous prix actuel) (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.5 : Stopper achats crypto (réinversion corrélation → double exposition) (1/3 runs)
🔴 sp500 : Prochaine publication CPI/Fed : si surprise hawkish, suspendre ETF Core et conserver cash (1/3 runs)
🔴 Si btc_price_eur ≤ 48000 : Stop achats BTC/ETH jusqu'au prochain run (cassure non contrôlée) (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Stop total crypto (risque crédit/stablecoin) (1/3 runs)
🔴 Si vix ≥ 30 : Suspendre ETF thématiques et crypto (1/3 runs)
🔴 Si dxy ≥ 103 : Suspendre accélérations crypto (drainage liquidité USD) (1/3 runs)
🔴 — : Publication inflation/Fed : si surprise hawkish, suspendre accélérations (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Stop achats crypto — stress stablecoins au-delà du bruit (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Stopper le DCA crypto jusqu'à confirmation SOPR/MVRV (1/3 runs)
🔴 Si vix ≥ 28 : Suspendre achats ETF — risque actions trop instable (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Interdire achat simultané crypto + equity au cycle suivant (1/3 runs)
🔴 Si contagion ≥ 40 : Stopper nouveaux achats crypto (passage HIGH) (1/3 runs)

CASH APRÈS EXÉCUTION : 16,153€ (0.0%)
ALLOCATIONS : Crypto 34.9% | ETF Core 11.8% | ETF Thématiques 1.5%
DISPERSION DES RUNS : Run1: 2,400€ — Run2: 3,200€ — Run3: 2,400€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Equilibre` (user `Equilibre`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 15%, reçu 0.0% — profil Equilibre
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 48.2%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 75.0% | 0.0% | 25.0% | 0.0% | 🔴 crypto_max, cash_min |
| Run2 | 15.3% | 0.0% | 6.4% | 2.4% | 🔴 cash_min |
| Run3 | 14.4% | 0.0% | 3.9% | 2.0% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*