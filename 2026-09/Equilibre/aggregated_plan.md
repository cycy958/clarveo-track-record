═══════════════════════════════════════════
  PLAN D'ACTION — 2026-09 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.70
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,750€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| EIMI | ACHETER | 750€ | 600–800€ | DCA | 3/3 |
| SWRD | ACHETER | 1,150€ | 600–1,600€ | DCA | 3/3 |
| XDWH | ACHETER | 850€ | 400–1,800€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si vix ≥ 22 : Suspendre les tranches ETF restantes — sortie nette de la zone calme (VIX 14,11, 5e percentile 90j) (1/3 runs)
🔴 Si us10y ≥ 5.00 : Suspendre SWRD, EIMI et XDWH — seuil abaissé de 5,20 pour agir avant réalisation complète du scénario taux (1/3 runs)
🔴 — : Publication CPI US de septembre : si surprise haussière avec tension sur les taux, suspendre les tranches S2-S4. Date à vérifier au calendrier officiel, non fournie par le rapport (1/3 runs)
🔴 Si us10y ≥ 5.10 : Suspendre les tranches DCA ETF restantes — scénario de repricing inflation/taux du RISK BRIEF Q3 (1/3 runs)
🔴 Si oil_wti ≥ 100 : Suspendre les tranches DCA ETF restantes — pétrole déjà au 96e percentile, +20.7% sur 30j (1/3 runs)
🔴 Si vix ≥ 28 : Suspendre les tranches DCA ETF restantes — doublement depuis 14.11, retour de la corrélation de stress (1/3 runs)
🔴 Si vix ≥ 22 : Suspendre les tranches ETF restantes et réévaluer le régime (1/3 runs)
🔴 Si oil_wti ≥ 100 : Suspendre les nouveaux achats ETF jusqu'à stabilisation du risque inflation (1/3 runs)
🔴 Si us10y ≥ 5.00 : Suspendre les renforcements Core et thématiques (1/3 runs)
🔴 Si funding_btc ≥ 20 : Suspendre le one-shot BTC conditionnel (1/3 runs)
🔴 — : Réunion FOMC de septembre : si message hawkish, suspendre S3-S4. Date à vérifier au calendrier officiel, non fournie par le rapport (1/3 runs)
🔴 Si contagion ≥ 40 : Suspendre toutes les tranches restantes et le one-shot BTC (1/3 runs)

CASH APRÈS EXÉCUTION : 13,003€ (52.3%)
ALLOCATIONS : Crypto 21.3% | ETF Core 19.8% | ETF Thématiques 6.7%
DISPERSION DES RUNS : Run1: 4,200€ — Run2: 1,600€ — Run3: 2,400€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Equilibre` (user `Equilibre`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

✅ **Plan agrégé conforme** aux contraintes V5.1 du profil.

- Crypto : 21.3% (plafond profil)
- Cash : 52.3% (plancher profil)

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 21.3% | 46.4% | 21.9% | 10.5% | ✅ |
| Run2 | 21.3% | 56.8% | 17.1% | 4.8% | ✅ |
| Run3 | 21.3% | 53.6% | 20.3% | 4.8% | ✅ |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*