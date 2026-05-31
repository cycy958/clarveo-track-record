# Patches runtime — TresOffensif — 2026-05

> Ce fichier documente les corrections appliquées au plan **runtime** déployé sur la VM pendant le mois, en dehors du plan IA scellé OpenTimestamps (`track_record_*.sha256.ots`).
>
> Le plan scellé reste l'engagement initial R3 du 1er du mois et n'est jamais modifié. Les patches ci-dessous corrigent des bugs détectés après scellement (anomalies de seuils, sémantique inversée, doublons exacts) sans toucher l'archive scellée.
>
> Pour comprendre la démarche complète, voir le README de ce dossier.

## Patches appliqués

### 2026-05-14 — Phase Y.1.b

Déduplication conservative des triggers (3 paires fusionnées : `vix above 25/22 → 22`, `oil_wti above 115/110 → 110`, `btc_nasdaq_corr above 0.97/0.90 → 0.90`). Le seuil retenu est le plus prudent.

