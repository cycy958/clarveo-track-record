# Profil Équilibré — juin 2026

Ce dossier contient le plan d'investissement du mois. Il a été scellé sur
Bitcoin via OpenTimestamps au moment de sa génération (run R1→R3), puis
publié ici un mois plus tard.

## Fichiers scellés (OpenTimestamps)

| Fichier | Description | SHA256 |
|---------|-------------|--------|
| `aggregated_plan.md` | Plan IA du mois | `8e31b95483c3221ccd81d3a303f001dee325eade2c412d1b4e3d5d164b66251b` |
| `dca_schedule_Equilibre.json` | Planning DCA hebdomadaire | `d0138bd246db0ac2061c3daa5382d049f374a9878ce6c1e56b3ea67cd1301253` |
| `active_triggers_Equilibre.json` | Seuils triggers PAUSE / ACCEL | `e42f7935e0783beb1ac5845a78dc647eaaf97c2f26acab1cd95d343e0f5140ed` |

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
- Total investi : 3 996,79 €
- Valeur des positions : 3 442,32 €
- Rendement : -13,87 % (DCA miroir : -1,14 %)
- Triggers déclenchés : —

## Suivi en direct

https://getclarveo.com/performance/
