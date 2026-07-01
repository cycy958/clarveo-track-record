# Profil Défensif — juin 2026

Ce dossier contient le plan d'investissement du mois. Il a été scellé sur
Bitcoin via OpenTimestamps au moment de sa génération (run R1→R3), puis
publié ici un mois plus tard.

## Fichiers scellés (OpenTimestamps)

| Fichier | Description | SHA256 |
|---------|-------------|--------|
| `aggregated_plan.md` | Plan IA du mois | `cc395bc193999a21748f558725c6f0189f8903e550caaf06ec509f0c20ea3d98` |
| `dca_schedule_Defensif.json` | Planning DCA hebdomadaire | `95c7cc7e34c523e2848c2d7ebb40173eb8f1e3e003a6d413303a2fb583bd0667` |
| `active_triggers_Defensif.json` | Seuils triggers PAUSE / ACCEL | `d2e1f2a171a93550f858791ac8112b833c6738de6792331f5fc83b9c259a2045` |

Le manifest `track_record_Defensif.sha256` reprend ces hashs au format `sha256sum -c`.

## Preuve OpenTimestamps

`track_record_Defensif.sha256.ots` ancre les hashs du manifest sur la blockchain Bitcoin.

### Vérifier localement

```bash
pip install opentimestamps-client

# 1. Intégrité des 3 fichiers contre le manifest
sha256sum -c track_record_Defensif.sha256

# 2. (optionnel) Récupérer la preuve Bitcoin complète
ots upgrade track_record_Defensif.sha256.ots

# 3. Vérifier la preuve contre le manifest
ots verify track_record_Defensif.sha256.ots track_record_Defensif.sha256
```

`ots verify` indique le bloc Bitcoin depuis lequel le manifest n'a pas
bougé. Le mois qui sépare la génération du plan de sa publication empêche
de le réécrire en fonction de ce qu'a fait le marché entre-temps.

## Résultats du mois

- Capital initial : 20 000,00 €
- Total investi : 3 699,15 €
- Valeur des positions : 3 513,62 €
- Rendement : -5,02 % (DCA miroir : +2,74 %)
- Triggers déclenchés : —

## Suivi en direct

https://getclarveo.com/performance/
