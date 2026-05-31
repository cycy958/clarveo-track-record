# Patches runtime — Offensif — 2026-05

> Ce fichier documente les corrections appliquées au plan **runtime** déployé sur la VM pendant le mois, en dehors du plan IA scellé OpenTimestamps (`track_record_*.sha256.ots`).
>
> Le plan scellé reste l'engagement initial R3 du 1er du mois et n'est jamais modifié. Les patches ci-dessous corrigent des bugs détectés après scellement (anomalies de seuils, sémantique inversée, doublons exacts) sans toucher l'archive scellée.
>
> Pour comprendre la démarche complète, voir le README de ce dossier.

## Patches appliqués

### 2026-05-11 — Phase O.2

Suppression du trigger `stablecoin_depeg below 0.999` (sémantique inversée). La condition `0.0 ≤ 0.999` étant toujours vraie, le profil était en PAUSE permanente depuis le 3 mai — faux positif structurel.

