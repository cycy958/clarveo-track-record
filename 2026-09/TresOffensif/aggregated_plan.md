═══════════════════════════════════════════
  PLAN D'ACTION — 2026-09 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.70
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,550€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 850€ | 600–1,200€ | DCA | 3/3 |
| DFEN | ACHETER | 100€ | 320–320€ | DCA | 1/3 |
| EIMI | ACHETER | 550€ | 400–600€ | DCA | 3/3 |
| ETH | ACHETER | 350€ | 200–400€ | DCA | 3/3 |
| SWRD | ACHETER | 150€ | 400–400€ | DCA | 1/3 |
| XDWH | ACHETER | 550€ | 400–800€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si vix ≥ 28 : Suspendre toutes les tranches restantes BTC, ETH et ETF (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Suspendre les achats crypto (1/3 runs)
🔴 Si funding_eth ≥ 25 : Suspendre les tranches ETH restantes (1/3 runs)
🔴 Si us10y ≥ 5.10 : Suspendre les tranches ETF restantes (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre les tranches restantes et réévaluer — entrée en volatilité élevée, proche du niveau J-180 de 26.64 (1/3 runs)
🔴 Si us10y ≥ 5.0 : Suspendre les tranches BTC/ETH — matérialise le risque de taux réels identifié par l'auditeur (1/3 runs)
🔴 Si gold_usd ≤ 3980 : Suspendre les tranches BTC/ETH — proxy avancé du risque BTC via corrélation 0.615 au 99e percentile (1/3 runs)
🔴 Si us10y ≥ 5.00 : Suspendre tous les nouveaux achats crypto et ETF — matérialisation du choc de taux réels (1/3 runs)
🔴 Si oil_wti ≥ 100 : Suspendre tous les nouveaux achats — vélocité pétrole déjà au 95e percentile 30j (1/3 runs)
🔴 Si funding_eth ≥ 15 : Suspendre les achats ETH — entrée en zone de stress du levier (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Suspendre les achats crypto — normalisation de la corrélation, perte de la diversification (1/3 runs)
🔴 Si gold_usd ≤ 3980 : Suspendre les achats crypto — vecteur de contagion or→BTC via corrélation 0.615 (1/3 runs)
🔴 — : FOMC 15-16 septembre 2026 (date à confirmer manuellement) : si ton hawkish, suspendre les tranches crypto restantes (1/3 runs)
🔴 Si contagion ≥ 40 : Suspendre tout nouveau déploiement jusqu'au retour sous 40 (1/3 runs)
🔴 Si contagion ≥ 80 : STOP total des nouveaux déploiements — seuil CRITICAL, garde-fou absolu (1/3 runs)

CASH APRÈS EXÉCUTION : 10,206€ (39.5%)
ALLOCATIONS : Crypto 45.2% | ETF Core 9.7% | ETF Thématiques 5.5%
DISPERSION DES RUNS : Run1: 2,000€ — Run2: 2,920€ — Run3: 2,600€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `TresOffensif` (user `TresOffensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

✅ **Plan agrégé conforme** aux contraintes V5.1 du profil.

- Crypto : 45.2% (plafond profil)
- Cash : 39.5% (plancher profil)

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 45.2% | 41.5% | 8.7% | 4.6% | ✅ |
| Run2 | 43.7% | 37.9% | 11.0% | 7.4% | ✅ |
| Run3 | 46.8% | 39.2% | 9.5% | 4.6% | ✅ |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*