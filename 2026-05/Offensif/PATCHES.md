# Corrections et précisions - Offensif - 2026-05

> Ce fichier liste les corrections et les précisions apportées après le scellement du plan de ce mois.
>
> Les fichiers scellés (`aggregated_plan.md`, `dca_schedule_<profil>.json`, `active_triggers_<profil>.json`) restent l'engagement d'origine. Ils ne sont jamais modifiés : une correction appliquée ensuite, ou une précision sur les données qui ont servi au plan, est notée ici, datée.
>
> Pour vérifier les fichiers scellés, voir le README de ce dossier.

## Détail

### 2026-05-11 - Phase O.2

Suppression du trigger `stablecoin_depeg below 0.999` (sémantique inversée). La condition `0.0 ≤ 0.999` étant toujours vraie, le profil était en PAUSE permanente depuis le 3 mai - faux positif structurel.

