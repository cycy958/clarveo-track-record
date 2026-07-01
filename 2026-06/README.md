# Track record — 2026-06

Plans d'investissement publiés le 2026-07-01 pour le mois 2026-06.

Cette publication intervient au minimum un mois après la génération
des plans (fenêtre de réserve obligatoire). Aucun contenu ne peut être
modifié a posteriori : le hash de chaque plan a été ancré sur la
blockchain Bitcoin via OpenTimestamps au moment du run R1→R3, soit
plusieurs semaines avant cette publication.

## Profils publiés

- `Defensif/`
- `Equilibre/`
- `Offensif/`
- `TresOffensif/`

## Comment vérifier l'authenticité

Chaque profil contient :

- `aggregated_plan.md` — plan détaillé issu du pipeline R1→R3
- `dca_schedule_<profile>.json` — planning DCA hebdomadaire
- `active_triggers_<profile>.json` — triggers conditionnels surveillés
- `track_record_<profile>.sha256` — hashes SHA256 des 3 fichiers ci-dessus
  au format `sha256sum -c`
- `track_record_<profile>.sha256.ots` — preuve OpenTimestamps ancrée sur
  la blockchain Bitcoin

### Étapes de vérification

```bash
# Installer le client OpenTimestamps
pip install opentimestamps-client

# Se placer dans le dossier d'un profil
cd <profile>/

# 1. Vérifier l'intégrité des 3 fichiers contre le manifest
sha256sum -c track_record_<profile>.sha256

# 2. (optionnel) Récupérer la preuve Bitcoin complète
ots upgrade track_record_<profile>.sha256.ots

# 3. Vérifier que la preuve correspond bien au manifest
ots verify track_record_<profile>.sha256.ots
```

La preuve `.ots` confirme que les hashes du manifest existaient bien dans
leur version exacte au moment où le pipeline R1→R3 les a soumis aux
calendars OpenTimestamps. La fenêtre de réserve d'un mois entre la
génération du plan et sa publication garantit qu'aucun plan ne peut
être ré-écrit a posteriori en fonction de la performance du marché.
