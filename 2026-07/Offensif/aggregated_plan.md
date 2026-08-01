═══════════════════════════════════════════
  PLAN D'ACTION — 2026-07 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.75
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,800€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BOTZ | ACHETER | 150€ | 100–200€ | DCA | 3/3 |
| BTC | ACHETER | 750€ | 700–800€ | DCA | 3/3 |
| CIBR | ACHETER | 150€ | 100–350€ | DCA | 2/3 |
| EIMI | ACHETER | 300€ | 300–300€ | DCA | 3/3 |
| ETH | ACHETER | 500€ | 450–600€ | DCA | 3/3 |
| SKYY | ACHETER | 200€ | 150–300€ | DCA | 3/3 |
| SWRD | ACHETER | 750€ | 600–900€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si funding_btc ≥ 15 : Suspendre achats BTC ; risque de squeeze de longs (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Stop achats crypto jusqu'à stabilisation (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Suspendre tous les achats crypto ; risque systémique (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Ne plus acheter crypto et equity la même semaine (1/3 runs)
🔴 Si dxy ≥ 103 : Suspendre achats EIMI + crypto de la semaine (headwind dollar) (1/3 runs)
🔴 Si vix ≥ 25 : Stopper achats ETF thématiques et crypto ; conserver le cash jusqu'au prochain run (1/3 runs)
🔴 Si funding_btc ≥ 15 : Suspendre achats BTC/ETH : risque de flush des longs trop élevé (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Ne plus acheter crypto et equity la même semaine ; priorité cash (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Stop crypto immédiat ; stress marché non compensé par le contrarien (1/3 runs)
🔴 gold_usd : Revue humaine avant tranche suivante : vérifier dislocation cross-asset / deleveraging forcé (1/3 runs)
🔴 Si funding_btc ≥ 15 : Suspendre achats BTC : rebond trop porté par le levier (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre crypto + ETF thématiques ; conserver core en cours (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Ne pas cumuler crypto + ETF thématiques : double exposition risk-on (1/3 runs)
🔴 — : CPI/NFP US : surprise inflation ou emploi fort → suspendre une semaine de DCA risqué (1/3 runs)
🔴 — : CPI US / FOMC juillet : si inflation réaccélère ou ton Fed hawkish, suspendre achats risk assets restants (1/3 runs)
🔴 Si contagion ≥ 40 : Suspendre tous les nouveaux achats crypto et ETF risqués (1/3 runs)
🔴 Si contagion ≥ 80 : Stop total nouveaux achats : risque systémique (1/3 runs)
🔴 Si contagion ≥ 40 : Suspendre achats crypto et ETF thématiques ; garder ETF Core défensif si VIX < 25 (1/3 runs)

CASH APRÈS EXÉCUTION : 11,806€ (0.0%)
ALLOCATIONS : Crypto 30.1% | ETF Core 10.9% | ETF Thématiques 4.6%
DISPERSION DES RUNS : Run1: 2,800€ — Run2: 3,000€ — Run3: 3,000€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Offensif` (user `Offensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 5%, reçu 0.0% — profil Offensif
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 45.6%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 30.7% | 0.0% | 9.8% | 4.4% | 🔴 cash_min |
| Run2 | 29.8% | 0.0% | 12.1% | 4.0% | 🔴 cash_min |
| Run3 | 29.8% | 0.0% | 10.7% | 5.4% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*