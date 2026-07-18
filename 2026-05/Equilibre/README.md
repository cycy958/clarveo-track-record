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

`track_record_Equilibre.sha256.ots` ancre les hashs du manifest `track_record_Equilibre.sha256` sur la blockchain Bitcoin. La preuve est autonome : elle se vérifie contre la blockchain seule, sans dépendre d'aucun service en ligne.

### Contrôler l'intégrité des fichiers

```bash
tr -d '\r' < track_record_Equilibre.sha256 | sha256sum -c -
```

Le `tr -d '\r'` neutralise les fins de ligne Windows du manifest. Chaque
fichier scellé doit afficher `OK`. Cette vérification ne dépend d'aucun
service extérieur et reste disponible en permanence.

### Vérifier l'ancrage Bitcoin

```bash
pip install opentimestamps-client
ots verify track_record_Equilibre.sha256.ots track_record_Equilibre.sha256
```

`ots verify` indique le bloc Bitcoin depuis lequel le manifest n'a pas bougé.
Le client `ots` est instable sous Windows.

### Vérificateur web (quand il est en ligne)

Vous pouvez aussi déposer `track_record_Equilibre.sha256.ots` avec le manifest
`track_record_Equilibre.sha256` sur https://opentimestamps.org/, qui confirme le
bloc Bitcoin en glisser-déposer sans rien installer. Ce service tiers connaît
des interruptions ; les deux vérifications ci-dessus, elles, restent
disponibles.

Le mois entre la génération du plan et sa publication interdit de le réécrire
selon le marché.

## Résultats du mois

- Capital initial : 20 000,00 €
- Total investi : 2 296,79 €
- Valeur des positions : 2 140,86 €
- Rendement : -6,79 % (DCA miroir : +1,51 %)
- Triggers déclenchés : —

## Suivi en direct

https://getclarveo.com/performance/
