# clarveo-track-record

Les plans d'investissement produits par [Clarveo](https://getclarveo.com), publiés
avec de quoi vérifier qu'ils n'ont pas été réécrits après coup.

Ce dépôt ne contient pas de résultats. Il contient les décisions et leurs preuves.
Les chiffres sont sur le site.

## Ce que vous trouvez ici

Un dossier par mois, et dans chacun un dossier par profil de risque.

```text
<mois>/                                  au format AAAA-MM
├── README.md
├── Defensif/
│   ├── aggregated_plan.md               le plan du mois, tel que produit
│   ├── dca_schedule_<profil>.json       les achats prévus, semaine par semaine
│   ├── active_triggers_<profil>.json    les seuils qui peuvent suspendre ou accélérer
│   ├── track_record_<profil>.sha256     l'empreinte des fichiers scellés
│   ├── track_record_<profil>.sha256.ots la preuve d'horodatage
│   ├── README.md                        le détail du dossier
│   └── PATCHES.md                       les correctifs appliqués après scellement
├── Equilibre/
├── Offensif/
└── TresOffensif/
```

Le plan, le calendrier d'achat et les seuils sortent du pipeline le jour où le
signal est produit. Les deux derniers fichiers sont écrits plus tard, et c'est
justement le sujet de la section suivante.

## Ce qui est scellé, et ce qui ne l'est pas

Tout n'est pas scellé, et je préfère le dire que le laisser découvrir.

**Le manifeste fait foi.** `track_record_<profil>.sha256` liste les fichiers
couverts par la preuve, et lui seul en décide. Ouvrez-le : ce que vous y lisez
est scellé, le reste ne l'est pas.

Les fichiers que j'écris après coup n'en font pas partie. Le README du dossier
et le journal des correctifs sont rédigés une fois le mois passé, donc les
inclure n'aurait aucun sens : ils n'existaient pas au moment du scellement.

Ça veut dire quelque chose de précis. Un correctif noté dans `PATCHES.md` n'est
pas couvert par la preuve, et il n'a pas à l'être : il documente ce qui a été
changé sur le système en cours de mois, pendant que le plan scellé, lui, ne
bouge pas. Si les deux racontaient la même chose, l'un des deux serait inutile.

## Vérifier une preuve

Trois façons de faire, de la plus simple à la plus technique. La première suffit
dans la plupart des cas.

### 1. Le vérificateur en ligne

Ouvrez [opentimestamps.org](https://opentimestamps.org/), onglet *Verify*, et
déposez-y les deux fichiers du dossier : le `.sha256.ots` et le `.sha256`.

Le site vous répond avec le bloc Bitcoin qui horodate le plan et sa date. Rien à
installer, et ça marche sur n'importe quel système.

Cette date est ce qui compte. Comparez-la au mois du dossier : elle doit tomber
pendant ce mois, alors que la publication ici a eu lieu après. C'est tout
l'argument, et il tient en une comparaison.

### 2. Contrôler que les fichiers n'ont pas bougé

Le vérificateur en ligne prouve la date du manifeste. Cette commande prouve que
les fichiers du dossier correspondent toujours à ce manifeste.

Placez-vous dans le dossier d'un profil :

```bash
tr -d '\r' < track_record_<profil>.sha256 | sha256sum -c -
```

Chaque fichier scellé doit afficher `OK`.

Le `tr -d '\r'` retire d'éventuelles fins de ligne Windows du manifeste. Il ne
change rien quand il n'y en a pas, donc cette forme fonctionne quel que soit le
fichier. Sans lui, la vérification peut échouer sur certains mois en signalant
des fichiers introuvables, alors que tout est intact.

Sous Windows, cette commande demande Git Bash ou WSL.

### 3. En ligne de commande, pour aller au bout

```bash
pip install opentimestamps-client
ots verify track_record_<profil>.sha256.ots track_record_<profil>.sha256
```

La sortie donne le même bloc Bitcoin que le vérificateur en ligne, avec une
vérification locale de la chaîne complète.

Le client `ots` est réputé instable sous Windows, où il échoue à l'import. Si
vous tombez dessus, la première méthode donne le même résultat sans installer
quoi que ce soit.

Vous n'aurez pas besoin de `ots upgrade`. Les preuves publiées ici sont déjà
ancrées quand elles arrivent dans ce dépôt : l'ancrage sur Bitcoin prend
quelques heures, et la publication attend bien plus longtemps que ça.

## Ce que la preuve démontre, et ce qu'elle ne démontre pas

Elle démontre qu'un fichier précis existait avant une date, et que personne ne
l'a modifié depuis. C'est une preuve d'antériorité, rien de plus.

Elle ne dit rien de la qualité du plan. Un plan scellé peut être mauvais, et un
plan mauvais reste scellé. Ce que la preuve empêche, c'est de le réécrire une
fois le résultat connu, ou de ne publier que les mois qui arrangent.

Autrement dit : elle ne vous demande pas de me faire confiance sur mes
décisions, elle vous permet de ne pas m'en croire sur parole quant à leur date.

## Pourquoi la publication a un mois de retard

Un plan est publié ici le mois suivant celui où il a été produit, jamais avant.

Ce délai est le cœur du dispositif. Publier en direct laisserait la possibilité
d'ajuster, de retirer, de reformuler. En publiant après, avec un horodatage
antérieur, la marge de manœuvre disparaît : le plan est daté avant que son
résultat soit connu.

## À propos d'OpenTimestamps

[OpenTimestamps](https://opentimestamps.org/) est un protocole d'horodatage
publié en 2016 par Peter Todd, qui ancre une empreinte de fichier dans la
blockchain Bitcoin.

Il ne demande aucune confiance envers Clarveo. La preuve se vérifie hors ligne
avec n'importe quelle implémentation du protocole, et elle reste valable aussi
longtemps que la blockchain Bitcoin existe.

## Les résultats

Ils ne sont pas ici, et c'est volontaire : ce dépôt porte les décisions, pas
leur performance. Duplique les chiffres à deux endroits et ils finiront par
diverger.

Rendements, pertes maximales et comparaison avec un investissement automatique :
[getclarveo.com/performance](https://getclarveo.com/performance/).

Le fonctionnement du système :
[getclarveo.com/methodologie](https://getclarveo.com/methodologie/).

## Disclaimer

Les plans publiés ici sont produits par un système algorithmique et ont une
portée générale. Ils ne constituent pas un conseil en investissement
personnalisé au sens de l'article L. 321-1 du Code monétaire et financier. Vous
restez seul responsable de vos décisions. Les performances passées, simulées ou
réelles, ne préjugent pas des performances futures.
