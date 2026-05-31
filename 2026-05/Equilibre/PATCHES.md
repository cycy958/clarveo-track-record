# Patches runtime — Equilibre — 2026-05

> Ce fichier documente les corrections appliquées au plan **runtime** déployé sur la VM pendant le mois, en dehors du plan IA scellé OpenTimestamps (`track_record_*.sha256.ots`).
>
> Le plan scellé reste l'engagement initial R3 du 1er du mois et n'est jamais modifié. Les patches ci-dessous corrigent des bugs détectés après scellement (anomalies de seuils, sémantique inversée, doublons exacts) sans toucher l'archive scellée.
>
> Pour comprendre la démarche complète, voir le README de ce dossier.

## Patches appliqués

### 2026-05-10 — Phase J'''.b

Seuil `stablecoin_depeg above 0.2` corrigé à `1.0` (unité harmonisée avec les autres profils). 0.2 déclenchait quasi-quotidiennement sur du bruit normal — faux positif.

