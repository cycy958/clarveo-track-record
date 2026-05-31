# Profil Équilibré — mai 2026

Ce dossier contient le plan d'investissement du mois. Il a été scellé sur
Bitcoin via OpenTimestamps au moment de sa génération (run R1→R3), puis
publié ici un mois plus tard.

## Fichiers scellés (OpenTimestamps)

| Fichier | Description | SHA256 |
|---------|-------------|--------|
| `aggregated_plan.md` | Plan IA du mois | `a0bf018242057b956ff3862c72f5aa2b200ec0525f3765dc453ad613932b7cf2` |
| `dca_schedule_Equilibre.json` | Planning DCA hebdomadaire | `ef1bdc4d7b617c0362588a120187fc3501072546ef5239c5ec7c82f3f77d9e30` |
| `active_triggers_Equilibre.json` | Seuils triggers PAUSE / ACCEL | `e5fe1ff13ffc39e5d50b29b4ee6f12405cf314325d5f3eae1a3cd91dab7a1b7c` |

Le manifest `track_record_Equilibre.sha256` reprend ces hashs au format `sha256sum -c`.

## Preuve OpenTimestamps

`track_record_Equilibre.sha256.ots` ancre les hashs du manifest sur la blockchain Bitcoin.

### Vérifier localement

```bash
pip install opentimestamps-client

# 1. Intégrité des 3 fichiers contre le manifest
sha256sum -c track_record_Equilibre.sha256

# 2. (optionnel) Récupérer la preuve Bitcoin complète
ots upgrade track_record_Equilibre.sha256.ots

# 3. Vérifier la preuve contre le manifest
ots verify track_record_Equilibre.sha256.ots track_record_Equilibre.sha256
```

`ots verify` indique le bloc Bitcoin depuis lequel le manifest n'a pas
bougé. Le mois qui sépare la génération du plan de sa publication empêche
de le réécrire en fonction de ce qu'a fait le marché entre-temps.

## Résultats du mois

- Capital initial : 20 000,00 €
- Total investi : 2 296,79 €
- Valeur des positions : 2 140,86 €
- Rendement : -6,79 % (DCA miroir : +1,51 %)
- Triggers déclenchés : —

## Suivi en direct

https://getclarveo.com/performance/
