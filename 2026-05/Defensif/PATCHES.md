# Patches runtime — Defensif — 2026-05

> Ce fichier documente les corrections appliquées au plan **runtime** déployé sur la VM pendant le mois, en dehors du plan IA scellé OpenTimestamps (`track_record_*.sha256.ots`).
>
> Le plan scellé reste l'engagement initial R3 du 1er du mois et n'est jamais modifié. Les patches ci-dessous corrigent des bugs détectés après scellement (anomalies de seuils, sémantique inversée, doublons exacts) sans toucher l'archive scellée.
>
> Pour comprendre la démarche complète, voir le README de ce dossier.

## Patches appliqués

### 2026-05-10 — Phase J'''.b

Seuil `btc_nasdaq_corr above 70.0` corrigé à `0.70` (format ratio Pearson [-1, 1], pas pourcentage). L'unité 70.0 ne pouvait jamais être atteinte donc le trigger était inactif — faux négatif structurel.

