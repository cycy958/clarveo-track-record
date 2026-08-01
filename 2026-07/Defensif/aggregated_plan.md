═══════════════════════════════════════════
  PLAN D'ACTION — 2026-07 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.72
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,300€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 150€ | 200–200€ | DCA | 2/3 |
| CSPX | ACHETER | 250€ | 300–400€ | DCA | 2/3 |
| DX2E | ACHETER | 150€ | 400–400€ | DCA | 1/3 |
| EIMI | ACHETER | 450€ | 400–500€ | DCA | 3/3 |
| SWRD | ACHETER | 1,050€ | 1,000–1,200€ | DCA | 3/3 |
| XDWS | ACHETER | 250€ | 100–400€ | DCA | 3/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 fear_greed : FOMC 28-29/07 : si hausse/ton hawkish, suspendre achats semaine 4 (proxy EVENT) (2/3 runs)
🔴 Si funding_btc ≥ 12 : Stop achats BTC — levier déjà surchauffé à 10.38% (1/3 runs)
🔴 Si btc_price_eur ≤ 52000 : Stop achats crypto — le rebond échoue (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre achats ETF + crypto restants (stress, profil défensif) (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Suspendre toute crypto — au-dessus du bruit normal 0.1-0.3% (1/3 runs)
🔴 Si rsi_xdwh ≥ 80 : Skip la tranche XDWH de la semaine — surachat aggravé (1/3 runs)
🔴 vix : (repère) marché calme confirmé pour poursuivre le DCA (1/3 runs)
🔴 Si vix ≥ 24 : Suspendre les achats ETF restants (retour zone J-90 24.17, rupture du calme) (1/3 runs)
🔴 Si funding_btc ≥ 12 : Interdire tout achat crypto (levier excessif au-dessus des 10.38% actuels) (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Suspendre double exposition actions/crypto (diversif insuffisante profil défensif) (1/3 runs)
🔴 Si vix ≥ 24 : Suspendre tous nouveaux achats ETF et crypto (1/3 runs)
🔴 Si dxy ≥ 105 : Suspendre achats actifs risqués (régime macro invalidé) (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Stop achats BTC, attendre stabilisation (1/3 runs)
🔴 Si funding_btc ≥ 15 : Suspendre achat BTC (levier trop encombré) (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Interdire achats simultanés crypto + equity (diversification insuffisante) (1/3 runs)

CASH APRÈS EXÉCUTION : 15,851€ (0.0%)
ALLOCATIONS : Crypto 4.7% | ETF Core 21.4% | ETF Thématiques 2.6%
DISPERSION DES RUNS : Run1: 3,200€ — Run2: 1,800€ — Run3: 2,000€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Defensif` (user `Defensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **2 violation(s) détectée(s)** (1 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] cash_min_pct: attendu >= 20%, reçu 0.0% — profil Defensif
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 28.7%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 5.0% | 0.0% | 22.6% | 5.0% | 🔴 cash_min |
| Run2 | 4.1% | 0.0% | 20.3% | 1.8% | 🔴 cash_min |
| Run3 | 5.0% | 0.0% | 21.2% | 0.9% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*