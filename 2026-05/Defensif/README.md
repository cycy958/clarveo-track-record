# Profil Défensif — mai 2026

Ce dossier contient le plan d'investissement du mois. Il a été scellé sur
Bitcoin via OpenTimestamps au moment de sa génération (run R1→R3), puis
publié ici un mois plus tard.

## Fichiers scellés (OpenTimestamps)

| Fichier | Description | SHA256 |
|---------|-------------|--------|
| `aggregated_plan.md` | Plan IA du mois | `200ba524ca3a56b47bb4e5dc79835943e3914569d6090990f7006cee6e4d97de` |
| `dca_schedule_Defensif.json` | Planning DCA hebdomadaire | `a1f593cfdf55fb449e5cda3ac0fa11d4934914957783a1e781311afa8a3f2f42` |
| `active_triggers_Defensif.json` | Seuils triggers PAUSE / ACCEL | `0978ec7ce79e60a96ce3d552f12246d0a8a3b7300ad6add14badc8b28e49edd0` |

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
- Total investi : 1 649,15 €
- Valeur des positions : 1 612,13 €
- Rendement : -2,25 % (DCA miroir : +4,39 %)
- Triggers déclenchés : —

## Suivi en direct

https://getclarveo.com/performance/
