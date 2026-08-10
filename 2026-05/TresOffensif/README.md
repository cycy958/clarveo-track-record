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

`track_record_TresOffensif.sha256.ots` ancre les hashs du manifest `track_record_TresOffensif.sha256` sur la blockchain Bitcoin.

### Vérifier la preuve (recommandé)

Déposez `track_record_TresOffensif.sha256.ots` sur https://opentimestamps.org/ avec le manifest
`track_record_TresOffensif.sha256`. Le site confirme le bloc Bitcoin qui horodate le plan, sans
rien installer, sur n'importe quel système.

### Contrôler l'intégrité des fichiers (optionnel)

```bash
tr -d '\r' < track_record_TresOffensif.sha256 | sha256sum -c -
```

Le `tr -d '\r'` retire d'éventuelles fins de ligne Windows du manifest. Il ne
change rien quand il n'y en a pas, donc cette forme fonctionne quel que soit le
fichier. Chaque fichier scellé doit afficher `OK`.

### Vérifier en ligne de commande (optionnel)

```bash
pip install opentimestamps-client
ots verify track_record_TresOffensif.sha256.ots track_record_TresOffensif.sha256
```

`ots verify` indique le bloc Bitcoin depuis lequel le manifest n'a pas bougé.
Le client `ots` est instable sous Windows : dans ce cas, utilisez le
vérificateur web ci-dessus. Le mois entre la génération du plan et sa
publication interdit de le réécrire selon le marché.

## Les résultats

Ils ne sont pas dans ce dépôt, qui porte les décisions et leurs preuves.
Rendements, pertes maximales et comparaison avec un investissement automatique :

https://getclarveo.com/performance/
