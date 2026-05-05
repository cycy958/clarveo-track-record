# clarveo-track-record

> **État au 5 mai 2026 : aucun mois encore publié.**
> La première publication aura lieu le **1er juin 2026** et contiendra
> les recommandations du mois de mai. Cette fenêtre de réserve d'un
> mois fait partie de la garantie de transparence : un signal ne peut
> pas être réécrit a posteriori en fonction de l'évolution du marché.
> Voir le calendrier ci-dessous.

Track record public et infalsifiable des recommandations algorithmiques
publiées par [Clarveo](https://getclarveo.com).

Chaque 1er du mois, ce dépôt reçoit l'intégralité des plans
d'investissement générés le mois précédent — pour les quatre profils
de risque publics — accompagnés des preuves cryptographiques permettant
à n'importe qui de vérifier qu'aucun plan n'a été modifié après coup.

Aucun contenu n'est ajouté en avance : la fenêtre de réserve d'un mois
entre la génération d'un plan et sa publication ici garantit qu'il
n'est pas possible de réécrire un signal en fonction de la performance
réelle du marché.

## Structure

```text
clarveo-track-record/
├── 2026-05/
│   ├── README.md                                  ← instructions de vérification du mois
│   ├── Defensif/
│   │   ├── aggregated_plan.md                     ← plan détaillé issu du pipeline R1→R3
│   │   ├── dca_schedule_Defensif.json             ← planning DCA hebdomadaire
│   │   ├── active_triggers_Defensif.json          ← triggers conditionnels surveillés
│   │   ├── track_record_Defensif.sha256           ← manifeste SHA-256 des 3 fichiers
│   │   └── track_record_Defensif.sha256.ots       ← preuve OpenTimestamps (Bitcoin)
│   ├── Equilibre/
│   ├── Offensif/
│   └── TresOffensif/
├── 2026-06/
└── ...
```

Chaque dossier de profil contient cinq fichiers : les trois fichiers
sources du run, un manifeste SHA-256 au format `sha256sum -c`, et la
preuve OpenTimestamps correspondante.

## Vérifier l'authenticité d'une recommandation

### 1. Installer le client OpenTimestamps

```bash
pip install opentimestamps-client
```

### 2. Vérifier l'intégrité des fichiers

Depuis le dossier d'un profil — par exemple `2026-05/Defensif/` :

```bash
sha256sum -c track_record_Defensif.sha256
```

La commande doit retourner trois lignes `OK` (une par fichier source).
Si l'un des fichiers a été altéré, la commande échouera.

### 3. Récupérer la preuve Bitcoin complète

Quand un plan est généré, sa preuve est initialement « pending » :
le hash a été soumis aux serveurs OpenTimestamps mais l'ancrage Bitcoin
prend ~24 h. Pour récupérer la preuve finale :

```bash
ots upgrade track_record_Defensif.sha256.ots
```

### 4. Vérifier la preuve

```bash
ots verify track_record_Defensif.sha256.ots
```

La sortie indique la date à laquelle le hash a été ancré sur la
blockchain Bitcoin. Cette date doit être **antérieure** à la date de
publication de ce dossier — c'est ce qui prouve que le contenu n'a pas
été modifié après publication.

### Vérificateur web

Si `ots` n'est pas disponible localement, le vérificateur officiel
fonctionne dans un navigateur :
[opentimestamps.org](https://opentimestamps.org/). Il suffit d'y
glisser-déposer un fichier `.sha256.ots`.

## À propos d'OpenTimestamps

[OpenTimestamps](https://opentimestamps.org/) est un protocole standard
publié en 2016 par Peter Todd. Il fournit un horodatage cryptographique
ancré sur la blockchain Bitcoin :

- **Décentralisé** : aucune autorité centrale, aucune confiance
  nécessaire envers Clarveo.
- **Vérifiable** : la preuve peut être validée hors-ligne par toute
  implémentation conforme du protocole.
- **Permanent** : tant que la blockchain Bitcoin existe, la preuve
  reste valide.

Concrètement, la preuve `.ots` démontre que le hash du manifeste
existait à un instant donné, dont la date est attestée par un bloc
Bitcoin. Combinée à `sha256sum -c`, elle prouve que les trois fichiers
du run R3 sont exactement ceux qui ont été générés à cette date.

## Calendrier de publication

| Date | Événement |
|------|-----------|
| 3 mai 2026 | Premier run public (4 profils) |
| 1er juin 2026 | Première publication ici (recommandations de mai) |
| 1er de chaque mois | Publication du mois précédent |

## Disclaimer

Les recommandations publiées ici sont générées par un système
algorithmique et ont une portée générale. Elles ne constituent pas un
conseil en investissement personnalisé au sens de l'article L. 321-1
du Code monétaire et financier. Vous êtes seul responsable de vos
décisions d'investissement. Les performances passées, simulées ou
réelles, ne préjugent pas des performances futures.

Pour plus de détails sur la méthodologie :
[getclarveo.com/methodologie](https://getclarveo.com/methodologie).
