# Profil Très Offensif — juin 2026

Ce dossier contient le plan d'investissement du mois. Il a été scellé sur
Bitcoin via OpenTimestamps au moment de sa génération (run R1→R3), puis
publié ici un mois plus tard.

## Fichiers scellés (OpenTimestamps)

| Fichier | Description | SHA256 |
|---------|-------------|--------|
| `aggregated_plan.md` | Plan IA du mois | `421e6139a04285225ed05e877024b9d04cc8912fc8226593ef53c3354f842c69` |
| `dca_schedule_TresOffensif.json` | Planning DCA hebdomadaire | `1ded350f1cd17891a662ddd83269083a75f2b8281ebd6292779fcd931f284dec` |
| `active_triggers_TresOffensif.json` | Seuils triggers PAUSE / ACCEL | `af0e7e4989f709fabdd93e41848d75115d8f437a5fdac842c25b16b9ef4dd37f` |

Le manifest `track_record_TresOffensif.sha256` reprend ces hashs au format `sha256sum -c`.

## Preuve OpenTimestamps

`track_record_TresOffensif.sha256.ots` ancre les hashs du manifest sur la blockchain Bitcoin.

### Vérifier localement

```bash
pip install opentimestamps-client

# 1. Intégrité des 3 fichiers contre le manifest
sha256sum -c track_record_TresOffensif.sha256

# 2. (optionnel) Récupérer la preuve Bitcoin complète
ots upgrade track_record_TresOffensif.sha256.ots

# 3. Vérifier la preuve contre le manifest
ots verify track_record_TresOffensif.sha256.ots track_record_TresOffensif.sha256
```

`ots verify` indique le bloc Bitcoin depuis lequel le manifest n'a pas
bougé. Le mois qui sépare la génération du plan de sa publication empêche
de le réécrire en fonction de ce qu'a fait le marché entre-temps.

## Résultats du mois

- Capital initial : 20 000,00 €
- Total investi : 6 293,95 €
- Valeur des positions : 5 306,13 €
- Rendement : -15,69 % (DCA miroir : -10,02 %)
- Triggers déclenchés : —

## Suivi en direct

https://getclarveo.com/performance/
