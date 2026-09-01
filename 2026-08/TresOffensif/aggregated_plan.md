═══════════════════════════════════════════
  PLAN D'ACTION — 2026-08 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.74
═══════════════════════════════════════════

ACHATS CE MOIS (total : 1,400€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 550€ | 450–750€ | DCA | 3/3 |
| ETH | ACHETER | 200€ | 200–400€ | DCA | 2/3 |
| SWRD | ACHETER | 350€ | 200–500€ | DCA | 3/3 |
| XDWH | ACHETER | 100€ | 100–150€ | DCA | 2/3 |
| XDWS | ACHETER | 200€ | 100–300€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si contagion ≥ 40 : Suspendre tous les nouveaux achats crypto (3/3 runs)
🔴 Si vix ≥ 25 : Suspendre toutes les tranches BTC et ETF restantes (1/3 runs)
🔴 Si us10y ≥ 5.10 : Suspendre BTC, SWRD et XDWS jusqu'à stabilisation des taux (1/3 runs)
🔴 Si funding_eth ≥ 20 : Suspendre toutes les tranches crypto restantes (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.5 : STOP total du déploiement crypto (1/3 runs)
🔴 Si us10y ≥ 5.10 : Suspendre les achats BTC, ETH et CNDX — matérialisation du scénario taux réels (angle mort ② R1) (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Suspendre les achats crypto — seuil très au-dessus du bruit actuel de 0.11% (1/3 runs)
🔴 Si funding_eth ≥ 15 : Suspendre les achats ETH restants — empilement de levier long (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre les tranches ETF et crypto restantes (1/3 runs)
🔴 Si us10y ≥ 5.00 : Suspendre SWRD, SKYY et ETH (1/3 runs)
🔴 Si dxy ≥ 103 : Suspendre SWRD, SKYY et les tranches crypto restantes (1/3 runs)
🔴 Si funding_eth ≥ 12 : Stopper toutes les tranches ETH (1/3 runs)
🔴 Si btc_price_eur ≤ 44000 : Suspendre les achats crypto 48h et réévaluer (-20 % depuis 54 954€) (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.5 : Suspendre toutes les tranches crypto restantes (1/3 runs)
🔴 Si contagion ≥ 80 : STOP total de tout nouveau déploiement (1/3 runs)

CASH APRÈS EXÉCUTION : 11,756€ (52.2%)
ALLOCATIONS : Crypto 36.1% | ETF Core 8.2% | ETF Thématiques 3.4%
DISPERSION DES RUNS : Run1: 1,550€ — Run2: 1,350€ — Run3: 1,450€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `TresOffensif` (user `TresOffensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

✅ **Plan agrégé conforme** aux contraintes V5.1 du profil.

- Crypto : 36.1% (plafond profil)
- Cash : 52.2% (plancher profil)

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 36.1% | 51.8% | 8.8% | 3.4% | ✅ |
| Run2 | 36.5% | 52.7% | 7.9% | 2.9% | ✅ |
| Run3 | 35.8% | 52.2% | 7.9% | 4.0% | ✅ |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*