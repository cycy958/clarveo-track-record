# Profil Très Offensif — mai 2026

Ce dossier contient le plan d'investissement du mois. Il a été scellé sur
Bitcoin via OpenTimestamps au moment de sa génération (run R1→R3), puis
publié ici un mois plus tard.

## Fichiers scellés (OpenTimestamps)

| Fichier | Description | SHA256 |
|---------|-------------|--------|
| `aggregated_plan.md` | Plan IA du mois | `febebd680a5970e096126f904f1573bd470fc5ecbb3e91283175034b0fe9ef0c` |
| `dca_schedule_TresOffensif.json` | Planning DCA hebdomadaire | `76c2e8dd2c50449d9d925cf897ab105c056ed6f0dfb13296cf167ad956992b6f` |
| `active_triggers_TresOffensif.json` | Seuils triggers PAUSE / ACCEL | `fdc41e481550dd5b0456c3ee07970277af4353825a54cfccbb0bd38b87c8456b` |

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
- Total investi : 3 993,95 €
- Valeur des positions : 3 714,40 €
- Rendement : -7,00 % (DCA miroir : -5,43 %)
- Triggers déclenchés : —

## Suivi en direct

https://getclarveo.com/performance/
