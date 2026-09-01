═══════════════════════════════════════════
  PLAN D'ACTION — 2026-08 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.78
═══════════════════════════════════════════

ACHATS CE MOIS (total : 1,050€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 50€ | 200–200€ | DCA | 1/3 |
| CSPX | ACHETER | 300€ | 250–400€ | DCA | 3/3 |
| SWRD | ACHETER | 350€ | 500–600€ | DCA | 2/3 |
| XDWH | ACHETER | 100€ | 100–150€ | DCA | 2/3 |
| XDWS | ACHETER | 250€ | 100–600€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si contagion ≥ 40 : Stopper tout déploiement restant jusqu'au prochain run mensuel (2/3 runs)
🔴 Si us10y ≥ 4.75 : Suspendre les tranches SWRD, CSPX et EIMI non exécutées et réévaluer le risque de duration (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre tous les achats restants pendant 48h et réévaluer la corrélation entre actifs (1/3 runs)
🔴 Si dxy ≥ 103 : Suspendre la ligne EIMI restante (sensibilité émergents au dollar) (1/3 runs)
🔴 Si us10y ≥ 5.00 : Suspendre toutes les tranches ETF et BTC restantes jusqu'à réévaluation du risque de duration (1/3 runs)
🔴 Si vix ≥ 28 : Suspendre les achats de la semaine et réévaluer la corrélation crypto-actions (1/3 runs)
🔴 Si btc_price_eur ≤ 48000 : Stopper les achats BTC et vérifier l'existence d'une liquidation systémique (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.50 : Suspendre la tranche BTC de la semaine — signal de stress de contrepartie crypto (1/3 runs)
🔴 us10y : Publication CPI US juillet : si surprise haussière confirmée par le 10Y, suspendre les ordres restants (1/3 runs)
🔴 Si us10y ≥ 4.75 : Suspendre toutes les tranches ETF restantes, réévaluer le risque de taux réels (1/3 runs)
🔴 Si oil_wti ≥ 95 : Suspendre le DCA CSPX, maintenir XDWS uniquement (1/3 runs)
🔴 Si gold_usd ≤ 3900 : Suspendre les tranches CSPX restantes, confirmation du repricing taux réels (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre les ordres market jusqu'à stabilisation (1/3 runs)

CASH APRÈS EXÉCUTION : 15,801€ (68.8%)
ALLOCATIONS : Crypto 4.9% | ETF Core 22.6% | ETF Thématiques 3.7%
DISPERSION DES RUNS : Run1: 1,300€ — Run2: 1,200€ — Run3: 1,000€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Defensif` (user `Defensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

✅ **Plan agrégé conforme** aux contraintes V5.1 du profil.

- Crypto : 4.9% (plafond profil)
- Cash : 68.8% (plancher profil)

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 4.6% | 68.2% | 23.9% | 3.3% | ✅ |
| Run2 | 5.5% | 68.6% | 22.8% | 3.1% | ✅ |
| Run3 | 4.6% | 69.5% | 21.0% | 4.8% | ✅ |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*