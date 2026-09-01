═══════════════════════════════════════════
  PLAN D'ACTION — 2026-08 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.77
═══════════════════════════════════════════

ACHATS CE MOIS (total : 1,400€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 500€ | 400–650€ | DCA | 3/3 |
| ETH | ACHETER | 100€ | 100–250€ | DCA | 2/3 |
| SWRD | ACHETER | 500€ | 350–700€ | DCA | 3/3 |
| XDWH | ACHETER | 100€ | 150–200€ | DCA | 2/3 |
| XDWS | ACHETER | 200€ | 200–350€ | DCA | 2/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si contagion ≥ 40 : Suspendre toutes les tranches régulières — passage de CALM à HIGH depuis un niveau actuel de 8/100 (3/3 runs)
🔴 Si vix ≥ 28 : Suspendre tous les nouveaux achats — entrée en volatilité élevée, antichambre du scénario VIX 32 du RISK BRIEF (1/3 runs)
🔴 Si us10y ≥ 5.0 : Suspendre SWRD et XDWS — scénario inflationniste avec pétrole au 96e percentile et duration sous pression (1/3 runs)
🔴 Si dxy ≥ 104 : Suspendre BTC et SWRD — couverture du risque de change EUR/USD non mesuré par le rapport (1/3 runs)
🔴 Si us10y ≥ 5.0 : Suspendre les achats ETF, réévaluer le choc pétrole-inflation (1/3 runs)
🔴 Si funding_eth ≥ 12 : Suspendre les achats ETH — accumulation de levier long (1/3 runs)
🔴 oil_wti : Surveillance humaine : transmission CPI, réévaluer les tranches ETF (1/3 runs)
🔴 Si us10y ≥ 5.00 : Suspendre les tranches SWRD, XDWH et XDWS : validation du scénario reflation « higher for longer », les actifs de duration longue encaissent en premier (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre toutes les tranches restantes : sortie du régime de volatilité calme et risque de recorrélation généralisée (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.60 : Suspendre les tranches crypto : la décorrélation au 2e percentile qui justifie la double exposition crypto + actions a disparu (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Suspendre BTC et ETH : écart très supérieur aux 0.11% actuels, signal de stress sur le collatéral (1/3 runs)
🔴 Si funding_eth ≥ 12.0 : Suspendre les tranches ETH : environ le double du funding actuel de 6.33%, confirmation d'un excès de levier long (1/3 runs)

CASH APRÈS EXÉCUTION : 11,406€ (50.7%)
ALLOCATIONS : Crypto 31.7% | ETF Core 11.8% | ETF Thématiques 5.7%
DISPERSION DES RUNS : Run1: 1,500€ — Run2: 1,250€ — Run3: 1,750€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Offensif` (user `Offensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

✅ **Plan agrégé conforme** aux contraintes V5.1 du profil.

- Crypto : 31.7% (plafond profil)
- Cash : 50.7% (plancher profil)

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 31.0% | 50.7% | 12.5% | 5.8% | ✅ |
| Run2 | 31.2% | 51.8% | 11.6% | 5.4% | ✅ |
| Run3 | 33.0% | 49.6% | 11.4% | 6.0% | ✅ |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*