# Profil Équilibré : octobre 2026

Ce dossier contient le plan d'investissement du mois. Il a été scellé sur
Bitcoin via OpenTimestamps au moment de sa génération (run R1→R3), puis
publié ici un mois plus tard.

## Fichiers scellés (OpenTimestamps)

| Fichier | Description | SHA256 |
|---------|-------------|--------|
| `aggregated_plan.md` | Plan IA du mois | `ee9b1518abe170332bf211419ad3c221f89a5129ec39db9b12ebfe5a448e6a1e` |
| `dca_schedule_Equilibre.json` | Planning DCA hebdomadaire | `249a12a3675847d938392a851f7f405ec7d2950b6e3f096fd3ea784ad99868f1` |
| `active_triggers_Equilibre.json` | Seuils triggers PAUSE / ACCEL | `25fff663efe82817004518d659f5f67011160dc0297c1c1cb2f40ebdb951bc20` |

Le manifest `track_record_Equilibre.sha256` reprend ces hashs au format `sha256sum -c`.

## Preuve OpenTimestamps

`track_record_Equilibre.sha256.ots` ancre les hashs du manifest `track_record_Equilibre.sha256` sur la blockchain Bitcoin.

### Vérifier la preuve (recommandé)

Déposez `track_record_Equilibre.sha256.ots` sur https://opentimestamps.org/ avec le manifest
`track_record_Equilibre.sha256`. Le site confirme le bloc Bitcoin qui horodate le plan, sans
rien installer, sur n'importe quel système.

### Contrôler l'intégrité des fichiers (optionnel)

```bash
tr -d '\r' < track_record_Equilibre.sha256 | sha256sum -c -
```

Le `tr -d '\r'` retire d'éventuelles fins de ligne Windows du manifest. Il ne
change rien quand il n'y en a pas, donc cette forme fonctionne quel que soit le
fichier. Chaque fichier scellé doit afficher `OK`.

### Vérifier en ligne de commande (optionnel)

```bash
pip install opentimestamps-client
ots verify track_record_Equilibre.sha256.ots track_record_Equilibre.sha256
```

`ots verify` indique le bloc Bitcoin depuis lequel le manifest n'a pas bougé.
Le client `ots` est instable sous Windows : dans ce cas, utilisez le
vérificateur web ci-dessus. Le mois entre la génération du plan et sa
publication interdit de le réécrire selon le marché.

## Les résultats

Ils ne sont pas dans ce dépôt, qui porte les décisions et leurs preuves.
Rendements, pertes maximales et comparaison avec un investissement automatique :

https://getclarveo.com/performance/
