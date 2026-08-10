# Profil Très Offensif — juillet 2026

Ce dossier contient le plan d'investissement du mois. Il a été scellé sur
Bitcoin via OpenTimestamps au moment de sa génération (run R1→R3), puis
publié ici un mois plus tard.

## Fichiers scellés (OpenTimestamps)

| Fichier | Description | SHA256 |
|---------|-------------|--------|
| `aggregated_plan.md` | Plan IA du mois | `e0640748f016ce8f9d12376afbddd287bc41da53394cd162f96835c363561111` |
| `dca_schedule_TresOffensif.json` | Planning DCA hebdomadaire | `4e82bf1e110365c3a89fa470cba27d0100a3856ed22452fbca35602dad451392` |
| `active_triggers_TresOffensif.json` | Seuils triggers PAUSE / ACCEL | `5f9b5ae348d986463b6db209916140875338ac81ccbcda9274535fa551037b81` |

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
