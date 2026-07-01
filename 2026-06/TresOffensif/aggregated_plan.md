═══════════════════════════════════════════
  PLAN D'ACTION — 2026-06 (NET ACHETEUR)
  Consensus : 2/2 runs, confiance 0.75
═══════════════════════════════════════════

ACHATS CE MOIS (total : 3,700€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 1,400€ | 1,000–1,850€ | DCA | 2/2 |
| DFEN | ACHETER | 150€ | 300–300€ | DCA | 1/2 |
| EIMI | ACHETER | 150€ | 300–300€ | DCA | 1/2 |
| ETH | ACHETER | 1,500€ | 1,400–1,550€ | DCA | 2/2 |
| SWRD | ACHETER | 500€ | 400–600€ | DCA | 2/2 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si vix ≥ 25 : Suspendre SWRD et réduire le DCA crypto restant de 50% (1/2 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Stop crypto immédiat (stress stablecoin sérieux) (1/2 runs)
🔴 Si btc_price_eur ≤ 48000 : Stop BTC/ETH restants jusqu'à stabilisation hebdomadaire (1/2 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Suspendre BTC/ETH (stress de peg réel). (1/2 runs)
🔴 Si vix ≥ 30 : Suspendre ETF Core/thématiques ET cryptos majors (choc VIX peut refermer la décorrélation BTC-SPX). (1/2 runs)
🔴 Si dxy ≥ 102 : Suspendre DCA crypto de base si surprise Fed/BCE hawkish confirmée (condition R3) (1/2 runs)
🔴 Si contagion ≥ 40 : Suspendre les achats crypto restants ; conserver le cash (1/2 runs)
🔴 Si contagion ≥ 60 : Suspendre tous achats crypto (risque systémique). (1/2 runs)

ACCÉLÉRATION (triggers) — majorité 2/3
───────────────────────────────────────
🟢 Si rsi_btc ≥ 30 : Ajouter 1 000€ crypto si contagion reste < 40 (1/2 runs)
🟢 Si vix ≤ 18 : Ajouter 500€ SWRD si les marchés actions se calment (1/2 runs)
🟢 Si btc_price_eur ≤ 50000 : Ajouter 1 000€ BTC/ETH si contagion <60 (seuil psychologique). (1/2 runs)
🟢 Si fear_greed ≤ 10 : Ajouter 1 000€ majors si stablecoins OK (panique extrême). (1/2 runs)
🟢 Si vix ≤ 18 : Ajouter 500€ ETF Core SWRD/EIMI (vol normalisée). (1/2 runs)

CASH APRÈS EXÉCUTION : 13,306€ (0.0%)
ALLOCATIONS : Crypto 29.5% | ETF Core 3.2% | ETF Thématiques 0.8%
DISPERSION DES RUNS : Run1: 3,000€ — Run2: 4,400€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `TresOffensif` (user `TresOffensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 5%, reçu 0.0% — profil TresOffensif
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 33.5%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 27.0% | 0.0% | 3.0% | 0.0% | 🔴 cash_min |
| Run2 | 32.0% | 0.0% | 3.5% | 1.5% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*