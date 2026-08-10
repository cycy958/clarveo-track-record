# Profil Offensif — mai 2026

Ce dossier contient le plan d'investissement du mois. Il a été scellé sur
Bitcoin via OpenTimestamps au moment de sa génération (run R1→R3), puis
publié ici un mois plus tard.

## Fichiers scellés (OpenTimestamps)

| Fichier | Description | SHA256 |
|---------|-------------|--------|
| `aggregated_plan.md` | Plan IA du mois | `fb527777cde2d8d0e8cd1cb7a2fa90c48b3c60fdd9c95632c2b091a9493cbad6` |
| `dca_schedule_Offensif.json` | Planning DCA hebdomadaire | `dd31adafb945de29f9a42565a3ee3b0d91aef037cee734c19fd10f6bc6ca23f3` |
| `active_triggers_Offensif.json` | Seuils triggers PAUSE / ACCEL | `50c39f5215107c8db0e690544e3013bcc0276f105859cc20d069999069909bc8` |

Le manifest `track_record_Offensif.sha256` reprend ces hashs au format `sha256sum -c`.

## Preuve OpenTimestamps

`track_record_Offensif.sha256.ots` ancre les hashs du manifest `track_record_Offensif.sha256` sur la blockchain Bitcoin.

### Vérifier la preuve (recommandé)

Déposez `track_record_Offensif.sha256.ots` sur https://opentimestamps.org/ avec le manifest
`track_record_Offensif.sha256`. Le site confirme le bloc Bitcoin qui horodate le plan, sans
rien installer, sur n'importe quel système.

### Contrôler l'intégrité des fichiers (optionnel)

```bash
tr -d '\r' < track_record_Offensif.sha256 | sha256sum -c -
```

Le `tr -d '\r'` retire d'éventuelles fins de ligne Windows du manifest. Il ne
change rien quand il n'y en a pas, donc cette forme fonctionne quel que soit le
fichier. Chaque fichier scellé doit afficher `OK`.

### Vérifier en ligne de commande (optionnel)

```bash
pip install opentimestamps-client
ots verify track_record_Offensif.sha256.ots track_record_Offensif.sha256
```

`ots verify` indique le bloc Bitcoin depuis lequel le manifest n'a pas bougé.
Le client `ots` est instable sous Windows : dans ce cas, utilisez le
vérificateur web ci-dessus. Le mois entre la génération du plan et sa
publication interdit de le réécrire selon le marché.

## Les résultats

Ils ne sont pas dans ce dépôt, qui porte les décisions et leurs preuves.
Rendements, pertes maximales et comparaison avec un investissement automatique :

https://getclarveo.com/performance/
