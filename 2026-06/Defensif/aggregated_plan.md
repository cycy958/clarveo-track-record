═══════════════════════════════════════════
  PLAN D'ACTION — 2026-06 (NET ACHETEUR)
  Consensus : 3/3 runs, confiance 0.75
═══════════════════════════════════════════

ACHATS CE MOIS (total : 2,500€)
───────────────────────────────────────
| Asset | Action | Montant | Min-Max | Méthode | Runs |
|-------|--------|---------|---------|---------|------|
| BTC | ACHETER | 450€ | 400–500€ | DCA | 3/3 |
| CSPX | ACHETER | 100€ | 300–300€ | DCA | 1/3 |
| EIMI | ACHETER | 500€ | 400–600€ | DCA | 3/3 |
| ETH | ACHETER | 200€ | 200–200€ | DCA | 3/3 |
| SWRD | ACHETER | 1,150€ | 1,000–1,200€ | DCA | 3/3 |
| XDWH | ACHETER | 100€ | 300–300€ | DCA | 1/3 |

STOP / PAUSE (triggers) — union des runs
───────────────────────────────────────
🔴 Si stablecoin_depeg ≥ 2.0 : Suspendre tous achats crypto + thématiques (canari systémique, ajout R3) (1/3 runs)
🔴 Si vix ≥ 28 : Suspendre CSPX, EIMI, XDWH, XDWS ; maintenir SWRD si contagion < 60 (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Stop achats BTC/ETH jusqu'au prochain run (éviter couteau qui tombe) (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Interdire achat simultané crypto + equity ; priorité cash (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Stop achats crypto, conserver uniquement ETF Core défensif (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Stop achats BTC/ETH, attendre stabilisation (1/3 runs)
🔴 Si vix ≥ 28 : Suspendre les achats ETF Core jusqu'au retour sous 25 (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.70 : Interdire achat simultané crypto + equity (1/3 runs)
🔴 — : Publications CPI/NFP/Fed : si surprise restrictive et DXY en forte hausse, suspendre les achats risqués (1/3 runs)
🔴 Si btc_price_eur ≤ 50000 : Suspendre achats BTC/ETH — cassure 50k€, invalidation du rebond actuel (1/3 runs)
🔴 Si vix ≥ 25 : Suspendre achats ETF Core — sortie du régime macro mécanique favorable (1/3 runs)
🔴 Si stablecoin_depeg ≥ 0.75 : Stop crypto — dépeg significatif des stablecoins majeurs (> bruit 0.1-0.3%) (1/3 runs)
🔴 Si dxy ≥ 102 : Suspendre achats risqués — choc de liquidité dollar confirmé (R1 angle mort #3) (1/3 runs)
🔴 Si btc_nasdaq_corr ≥ 0.5 : Suspendre achats crypto — re-corrélation actions, perte du coussin de découplage (R1 angle mort #2) (1/3 runs)
🔴 vix : Avant CPI/NFP/FOMC : ne pas accélérer si VIX monte ou US10Y en forte tension (1/3 runs)
🔴 Si contagion ≥ 60 : Suspendre achats crypto + thématiques ; ne garder que DCA Core défensif si VIX < 28 (1/3 runs)
🔴 Si contagion ≥ 40 : Suspendre achats crypto — passage ELEVATED → HIGH (1/3 runs)
🔴 Si contagion ≥ 60 : Suspendre tous les achats crypto et ETF thématiques (1/3 runs)

CASH APRÈS EXÉCUTION : 16,851€ (0.0%)
ALLOCATIONS : Crypto 12.0% | ETF Core 33.9% | ETF Thématiques 0.8%
DISPERSION DES RUNS : Run1: 3,000€ — Run2: 2,400€ — Run3: 2,200€
═══════════════════════════════════════════

## [VALIDATION_V5_1]

*Audit automatique des contraintes V5.1 pour le profil `Defensif` (user `Defensif`)*

### 1. Plan agrégé (post 2/3 vote + moyenne)

⚠️ **3 violation(s) détectée(s)** (2 erreur(s), 1 warning(s)) — à arbitrer par l'utilisateur final.

- [ERROR] crypto_max_pct: attendu <= 10%, reçu 12.0% — profil Defensif
- [ERROR] cash_min_pct: attendu >= 20%, reçu 0.0% — profil Defensif
- [WARNING] allocation_sum: attendu 100.0% (+/- 0.5), reçu 46.7%

### 2. Validation des runs individuels

| Run | Crypto | Cash | Core | Them | Violations |
|-----|-------:|-----:|-----:|-----:|------------|
| Run1 | 5.2% | 0.0% | 14.3% | 2.4% | 🔴 cash_min |
| Run2 | 25.0% | 0.0% | 75.0% | 0.0% | 🔴 crypto_max, cash_min |
| Run3 | 5.7% | 0.0% | 12.4% | 0.0% | 🔴 cash_min |

> *Note : le vote direction (2/3 majorité) et la moyenne des montants sont indépendants de la conformité V5.1 — un run en violation de contrainte peut quand même contribuer au plan agrégé.*