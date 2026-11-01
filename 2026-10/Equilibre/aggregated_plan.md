═══════════════════════════════════════════
  PLAN D'ACTION — 2026-10 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.70
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,500€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER (minoritaire, non retenue) | 150€ | 400–400€ | DCA | 1/3 |
| EIMI | ACHETER | 700€ | 500–1,000€ | DCA | 3/3 |
| SWRD | ACHETER | 650€ | 400–800€ | DCA | 3/3 |
| XDWH | ACHETER | 750€ | 600–1,000€ | DCA | 3/3 |
| XDWS | ACHETER | 250€ | 400–400€ | DCA | 2/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 — : 27-29 octobre 2026 : FOMC puis BCE, taux longs, dollar, volatilité (2/3 runs)
🔴 Si us10y ≥ 5.55 : TOUS : prolongation du signal taux extrême vers le scénario de stress 5.6-5.75% (1/3 runs) — effet retenu : suspendre tous les achats
🔴 Si vix ≥ 25 : TOUS : sortie du régime de volatilité normale (1/3 runs) — effet retenu : suspendre tous les achats
🔴 Si dxy ≥ 104 : EIMI : dollar fort pénalisant les émergents (1/3 runs) — effet retenu : alerte seule
🔴 🔔 Si funding_btc ≥ 15 : Levier crypto excessif, risque de liquidations sur les positions BTC/ETH détenues (1/3 runs) — effet retenu : alerte seule
🔴 🔔 Si btc_nasdaq_corr ≥ 0.70 : Perte du bénéfice de diversification crypto-actions (1/3 runs) — effet retenu : alerte seule
🔴 🔔 Si dxy ≤ 100 : Disparition du coussin dollar si les taux US restent élevés (scénario double peine) (1/3 runs) — effet retenu : alerte seule
🔴 Si us10y ≥ 5.60 : EIMI, SWRD, XDWH, XDWS : poursuite du choc de taux (+31 pb depuis 5.29%) (1/3 runs) — effet retenu : suspendre tous les achats
🔴 Si vix ≥ 25 : EIMI, SWRD, XDWH, XDWS : sortie du régime de volatilité calme (1/3 runs) — effet retenu : suspendre tous les achats
🔴 🔔 Si btc_nasdaq_corr ≥ 0.70 : Nouvelle dégradation de la diversification crypto/actions (actuel 0.49) (1/3 runs) — effet retenu : alerte seule
🔴 🔔 Si dxy ≤ 98 : Rebond EUR/USD vers ~1.18 qui pénalise en EUR les positions US et la crypto (1/3 runs) — effet retenu : alerte seule
🔴 🔔 Si funding_btc ≥ 20 : Excès de levier long sur BTC, risque de flush (actuel 7.64%, MA7 3.35%) (1/3 runs) — effet retenu : alerte seule
🔴 — : 7 octobre 2026 : minutes de la Fed, réaction du US10Y (1/3 runs)
🔴 Si us10y ≥ 5.8 : TOUS : repricing de +50 pb, scénario du stress test R1 (1/3 runs) — effet retenu : suspendre tous les achats
🔴 Si vix ≥ 30 : TOUS : zone de panique, attendre la stabilisation (1/3 runs) — effet retenu : suspendre tous les achats
🔴 Si funding_btc ≥ 15 : BTC : levier long environ 2× le niveau actuel déjà élevé (1/3 runs) — effet retenu : alerte seule
🔴 Si rsi_btc ≥ 75 : BTC : surachat fort combiné au levier, risque de purge (1/3 runs) — effet retenu : alerte seule
🔴 🔔 Si btc_nasdaq_corr ≥ 0.70 : Crypto et actions deviennent un seul facteur de risque (1/3 runs) — effet retenu : alerte seule
🔴 🔔 Si dxy ≥ 105 : Bascule d'un critère Risk-On, à réévaluer au run suivant (1/3 runs) — effet retenu : alerte seule
🔴 — : NFP 2 octobre 2026 : réaction du 10Y vs 5.29% avant S1 (1/3 runs)
🔴 — : Minutes Fed 7 octobre 2026 : ton sur les taux (1/3 runs)
🔴 — : BCE 28-29 octobre 2026 : ton monétaire, ETF européens et défensifs (1/3 runs)
🔴 Si contagion ≥ 40 : TOUS : stress systémique crédit/stablecoins (zone HIGH) (1/3 runs) — effet retenu : suspendre tous les achats
🔴 Si contagion ≥ 80 : TOUS : stress systémique, aucun déploiement (1/3 runs) — effet retenu : suspendre tous les achats

CASH APRÈS EXÉCUTION : 11,503€ (43.5%)
ALLOCATIONS : Crypto 22.3% | ETF Core 24.2% | ETF Thématiques 10.0%
DISPERSION DES RUNS : Run1: 2,300€ — Run2: 2,000€ — Run3: 3,200€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Equilibre` (user `Equilibre`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

✅ **Plan agrégé conforme** aux contraintes V5.1 du profil.

- Crypto : 22.3% (plafond profil)
- Cash : 43.5% (plancher profil)

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 21.8% | 44.3% | 24.0% | 10.0% | ✅ |
| Run2 | 21.8% | 45.4% | 22.8% | 10.0% | ✅ |
| Run3 | 23.3% | 40.9% | 25.9% | 10.0% | ✅ |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*