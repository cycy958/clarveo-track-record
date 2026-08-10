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
