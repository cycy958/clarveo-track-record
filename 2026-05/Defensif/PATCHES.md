# Corrections et précisions - Defensif - 2026-05

> Ce fichier liste les corrections et les précisions apportées après le scellement du plan de ce mois.
>
> Les fichiers scellés (`aggregated_plan.md`, `dca_schedule_<profil>.json`, `active_triggers_<profil>.json`) restent l'engagement d'origine. Ils ne sont jamais modifiés : une correction appliquée ensuite, ou une précision sur les données qui ont servi au plan, est notée ici, datée.
>
> Pour vérifier les fichiers scellés, voir le README de ce dossier.

## Détail

### 2026-05-10 - Phase J'''.b

Seuil `btc_nasdaq_corr above 70.0` corrigé à `0.70` (format ratio Pearson [-1, 1], pas pourcentage). L'unité 70.0 ne pouvait jamais être atteinte donc le trigger était inactif - faux négatif structurel.

