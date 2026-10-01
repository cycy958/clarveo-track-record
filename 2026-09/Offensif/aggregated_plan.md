═══════════════════════════════════════════
  PLAN D'ACTION — 2026-09 (NET ACHETEUR)
  Consensus : 2/2 runs, confiance 0.69
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,900€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 400€ | 400–400€ | DCA | 2/2 |
| CSPX | ACHETER | 300€ | 600–600€ | DCA | 1/2 |
| EIMI | ACHETER | 1,000€ | 950–1,000€ | DCA | 2/2 |
| SWRD | ACHETER | 800€ | 600–950€ | DCA | 2/2 |
| XDWH | ACHETER | 400€ | 400–450€ | DCA | 2/2 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si vix ≥ 28 : Suspendre le DCA restant — niveau du J-180 (26.64), stress test R1 ① (1/2 runs)
🔴 Si us10y ≥ 5.25 : Suspendre les achats ETF — scénario inflation/taux du stress test R1 ③ (1/2 runs)
🔴 Si fear_greed ≥ 85 : Suspendre les achats crypto — avidité extrême (1/2 runs)
🔴 Si funding_btc ≥ 25 : Suspendre le DCA BTC — empilement de levier long, signal R1 ③ (1/2 runs)
🔴 Si dxy ≥ 105 : Suspendre achats crypto et ETF — choc FX sur ~70% du portefeuille investi (1/2 runs)
🔴 Si fear_greed ≥ 80 : Suspendre les tranches BTC restantes : entrée en avidité extrême (1/2 runs)
🔴 Si funding_btc ≥ 15 : Suspendre les tranches BTC restantes : accumulation de levier long (1/2 runs)
🔴 Si mvrv ≥ 2.60 : Suspendre les tranches BTC restantes : base de coût on-chain dégradée (1/2 runs)
🔴 Si btc_price_eur ≤ 55000 : Stopper le DCA BTC : cassure sous la zone J-30 convertie (55 819€) (1/2 runs)
🔴 Si vix ≥ 28.5 : Suspendre toutes les nouvelles tranches : scénario de stress du RISK BRIEF (1/2 runs)
🔴 Si us10y ≥ 5.20 : Suspendre toutes les nouvelles tranches : rupture du narratif de détente monétaire (1/2 runs)
🔴 Si contagion ≥ 80 : Suspendre tout nouveau déploiement — seuil CRITICAL du garde-fou absolu (1/2 runs)

ACCÉLÉRATION (triggers) — majorité 2/3
───────────────────────────────────────
🟢 Si btc_price_eur ≤ 64000 : Avancer une tranche BTC de 100€ si aucun PAUSE actif : repli de 7% entre J-7 et J-30 convertis (1/2 runs)
🟢 Si vix ≥ 20 : Avancer une tranche SWRD et EIMI de 100€ chacune tant que VIX reste sous 28.5 : repli equity exploitable (1/2 runs)
🟢 Si btc_price_eur ≤ 56000 : Déployer 600€ additionnels sur BTC si contagion < 80 — repli vers l'ancrage J-30 (64 665$ ÷ 1.1585) (1/2 runs)

CASH APRÈS EXÉCUTION : 9,506€ (37.2%)
ALLOCATIONS : Crypto 37.6% | ETF Core 18.4% | ETF Thématiques 6.8%
DISPERSION DES RUNS : Run2: 3,000€ — Run3: 2,750€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Offensif` (user `Offensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

✅ **Plan agrégé conforme** aux contraintes V5.1 du profil.

- Crypto : 37.6% (plafond profil)
- Cash : 37.2% (plancher profil)

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run2 | 37.6% | 36.8% | 19.0% | 6.7% | ✅ |
| Run3 | 37.6% | 37.7% | 17.8% | 6.8% | ✅ |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*