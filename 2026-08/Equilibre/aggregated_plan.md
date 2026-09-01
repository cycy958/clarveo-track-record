═══════════════════════════════════════════
  PLAN D'ACTION — 2026-08 (NET ACHETEUR)
  Consensus : 2/2 runs, confiance 0.77
═══════════════════════════════════════════

ACHATS CE MOIS (total : 1,500€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 300€ | 250–300€ | DCA | 2/2 |
| CNDX | ACHETER | 200€ | 150–300€ | DCA | 2/2 |
| EIMI | ACHETER | 100€ | 250–250€ | DCA | 1/2 |
| ETH | ACHETER | 100€ | 150–150€ | DCA | 1/2 |
| SWRD | ACHETER | 500€ | 500–500€ | DCA | 2/2 |
| XDWH | ACHETER | 150€ | 100–200€ | DCA | 2/2 |
| XDWS | ACHETER | 150€ | 100–200€ | DCA | 2/2 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si us10y ≥ 5.00 : Suspendre les achats CNDX — matérialisation du repricing de duration (4,68% actuellement) (1/2 runs)
🔴 Si oil_wti ≥ 95 : Suspendre les achats CNDX et SWRD — prolongation du choc inflationniste amont (84,67 actuellement) (1/2 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Suspendre tous les achats crypto — écart très au-dessus du bruit naturel de 0,1 à 0,3% (1/2 runs)
🔴 Si funding_eth ≥ 25 : Suspendre tous les achats crypto — risque de cascade de liquidations non mesurable sans open interest (1/2 runs)
🔴 — : Run mensuel du 6 septembre 2026 : réévaluer flux ETF spot BTC, pétrole, US10Y, MACD daily et publication CPI (1/2 runs)
🔴 Si vix ≥ 25 : Suspendre toutes les tranches restantes — rupture nette vs snapshots 12 mois compris entre 16,18 et 18,69 (1/2 runs)
🔴 Si us10y ≥ 5.00 : Suspendre CNDX et les achats crypto — seuil psychologique à 32 pb du niveau actuel de 4,68% (1/2 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Suspendre BTC et ETH — dépasse largement le bruit actuel de 0,05 à 0,11% (1/2 runs)
🔴 Si oil_wti ≥ 95 : Suspendre les tranches CNDX et EIMI restantes — confirmation du pass-through inflationniste (1/2 runs)
🔴 us10y : Publication CPI US : si surprise haussière confirmée par US10Y > 4,80%, réévaluation manuelle des tranches restantes (1/2 runs)
🔴 Si contagion ≥ 40 : Suspendre les achats BTC — entrée en régime HIGH (8/100 actuellement) (1/2 runs)

ACCÉLÉRATION (triggers) — majorité 2/3
───────────────────────────────────────
🟢 Si mvrv ≤ 1.10 : Achat BTC one-shot 300€ — rapprochement de la zone de capitulation (1,20 actuellement) (1/2 runs)
🟢 Si fear_greed ≤ 15 : Achat BTC one-shot 300€ — vraie dislocation de sentiment, distincte de la peur stationnaire actuelle à 27 (1/2 runs)
🟢 Si rsi_cndx ≤ 30 : Achat CNDX one-shot 200€ — seuil de forte survente du rapport (38 actuellement) (1/2 runs)
🟢 Si fear_greed ≤ 20 : Avancer les tranches BTC/ETH restantes, budget crypto plafonné à 400€ (1/2 runs)
🟢 Si rsi_CNDX ≤ 32 : Avancer la tranche CNDX de semaine 4, budget plafonné à 150€ (1/2 runs)
🟢 Si mvrv ≤ 1.00 : Avancer les tranches crypto restantes, budget crypto plafonné à 400€ (1/2 runs)

CASH APRÈS EXÉCUTION : 14,753€ (65.2%)
ALLOCATIONS : Crypto 17.8% | ETF Core 13.5% | ETF Thématiques 3.5%
DISPERSION DES RUNS : Run1: 1,500€ — Run3: 1,500€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Equilibre` (user `Equilibre`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

✅ **Plan agrégé conforme** aux contraintes V5.1 du profil.

- Crypto : 17.8% (plafond profil)
- Cash : 65.2% (plancher profil)

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 17.5% | 65.2% | 13.3% | 4.0% | ✅ |
| Run3 | 18.0% | 65.2% | 13.7% | 3.1% | ✅ |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*