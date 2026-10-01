═══════════════════════════════════════════
  PLAN D'ACTION — 2026-09 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.74
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,250€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| CSPX | ACHETER | 350€ | 400–600€ | DCA | 2/3 |
| EIMI | ACHETER | 800€ | 400–1,200€ | DCA | 3/3 |
| ETH | VENDRE | 100€ | 130–150€ | DCA | 2/3 |
| SWRD | ACHETER | 600€ | 600–1,200€ | DCA | 2/3 |
| XDWH | ACHETER | 400€ | 200–600€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si us10y ≥ 5.00 : Suspendre les tranches ETF restantes — seuil psychologique précédant le scénario de stress 5,20% du RISK BRIEF (1/3 runs)
🔴 Si oil_wti ≥ 100 : Suspendre les nouveaux achats actions — confirmerait la prolongation du choc inflationniste déjà à +20,3% sur 30j (1/3 runs)
🔴 Si vix ≥ 22 : Suspendre les tranches restantes et réévaluer le régime — rupture nette du calme actuellement pricé à 14,15 (1/3 runs)
🔴 Si gold_usd ≤ 4100 : Neutraliser le trigger d'achat BTC — cassure du trade de couverture monétaire qui porte la crypto (corr BTC-GOLD 0,615, 99e pct) (1/3 runs)
🔴 Si funding_btc ≥ 20 : Neutraliser le trigger d'achat BTC — doublement du funding vs 9,74% actuel signale une cascade de liquidations, pas un point d'entrée (1/3 runs)
🔴 Si us10y ≥ 5.00 : Suspendre le DCA ETF Core restant, réévaluer le risque duration (1/3 runs)
🔴 Si oil_wti ≥ 95 : Suspendre le DCA ETF Core restant jusqu'à réévaluation inflation (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre le DCA ETF Core restant (1/3 runs)
🔴 Si vix ≥ 22 : Suspendre les tranches ETF restantes — entrée en zone de volatilité élevée, réaction anticipée pour profil Défensif (1/3 runs)
🔴 Si us10y ≥ 5.10 : Suspendre les nouveaux achats equity et réévaluer le régime — seuil de rupture identifié par le RISK BRIEF (1/3 runs)
🔴 Si oil_wti ≥ 100 : Suspendre XDWH et réévaluer le Core — poursuite du choc pétrolier à +20.3%/30j, 96e percentile (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.5 : Suspendre ACCEL crypto et tranches DCA restantes — capteur direct de stress de liquidité, indice de contagion non fiable (1/3 runs)
🔴 — : Publication du CPI US d'août : si elle confirme le choc inflationniste avec pétrole et taux longs élevés, suspendre le DCA restant (1/3 runs)
🔴 Si contagion ≥ 40 : Suspendre tous les achats restants (1/3 runs)

CASH APRÈS EXÉCUTION : 14,551€ (60.8%)
ALLOCATIONS : Crypto 5.6% | ETF Core 28.4% | ETF Thématiques 5.1%
DISPERSION DES RUNS : Run1: 2,270€ — Run2: 1,050€ — Run3: 2,800€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Defensif` (user `Defensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

✅ **Plan agrégé conforme** aux contraintes V5.1 du profil.

- Crypto : 5.6% (plafond profil)
- Cash : 60.8% (plancher profil)

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 5.4% | 59.9% | 28.7% | 6.0% | ✅ |
| Run2 | 5.3% | 64.9% | 25.4% | 4.3% | ✅ |
| Run3 | 6.0% | 57.7% | 31.2% | 5.1% | ✅ |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*