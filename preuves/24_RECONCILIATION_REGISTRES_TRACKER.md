# Réconciliation des registres et trackers — décision de version

## Décision de travail
Pour la phase en cours, l’étendue active est **P001–P1000**, conformément au registre complémentaire `23_REGISTRE_PROPHETIES_7.md`, qui contient P976–P1000, et à l’`INDEX_GENERAL.html` qui annonce 1000 entrées. P975 n’est donc pas la dernière entrée. P976–P980 sont désormais rédigées dans `phase10/FICHES_P976-P980.html`.

## Versions documentaires

| Document | Contenu observé | Traitement |
|---|---|---|
| `16_REGISTRE_PROPHETIES.md` à `21_REGISTRE_PROPHETIES_6.md` | Séries successives, avec plages qui se recoupent. La partie 6 présente P975 comme borne finale de sa version. | Conserver comme historique des versions; ne pas additionner les références répétées pour compter les entrées. |
| `23_REGISTRE_PROPHETIES_7.md` | Complément P976–P1000; indique que le registre couvre P001–P1000. | Source de vérité actuelle pour l’extension finale, en complément de la partie 6. |
| `INDEX_GENERAL.html` | Annonce 1000 entrées et classe notamment Juges P976–P980, Marc P981–P993, Colossiens P994, Jean P995–P1000. | Index de repérage, pas preuve d’existence d’une fiche détaillée. Vérifier le décalage entre les parties 21 et 23. |
| `phase9/00_WORKFLOW_PHASE9.md` | Tracker historique; contient les lots P506–P975 et, en fin de document, une conclusion erronée disant que P975 clôt le registre et qu’il ne faut pas inventer P976. Numéros de vagues non monotones/répétés. | Garder la trace de l’erreur; la conclusion est supersédée par le registre 23 et l’audit. Les vagues ne doivent pas servir de numérotation canonique. |
| `phase10/00_WORKFLOW_PHASE10.md` et `phase10/01_TRACKER_P976-P1000.md` | Machine à états et suivi actualisé de la phase d’achèvement. | Tracker opérationnel courant pour P976–P1000; les numéros de lots sont indépendants des vagues historiques phase 9. |

## Correction explicite du bloc de clôture de phase 9
Le bloc de phase 9 qui disait « Le registre numéroté s’achève à P975. Ne pas inventer P976 » est **invalidé par vérification** : le complément `23_REGISTRE_PROPHETIES_7.md` liste P976–P1000. Le journal de phase 9 est conservé pour la traçabilité, mais cette ancienne phrase ne constitue plus un état courant. Le statut « PUBLIÉ » de P975 reste valide pour la fiche P975; seule l’affirmation qu’il s’agissait de la dernière entrée est remplacée.

## Chemins de fichiers
Les chemins de type `../FICHES_….html` des journaux de phase 9 sont relatifs au dossier `preuves/phase9`; plusieurs exemples (notamment vagues P506–P517) ont été résolus depuis ce répertoire et existent. Ne pas les corriger en retirant `../` sans changer de répertoire de base. Pour la phase 10, les fiches HTML sont dans `preuves/phase10`; les chemins `../images/...` et `../audio/...` pointent donc vers les sous-dossiers médias de `preuves`.

## Couverture des fiches : règles pour le tableau maître
Le fichier `MASTER_ID_FICHES.csv` contient exactement une ligne par P001–P1000. Il distingue :
- **FICHE REPÉRÉE** : fichier de fiche détaillée associé localement, ou lot documenté dans le workflow et fichier correspondant existant;
- **FICHE PUBLIÉE — phase 10** : fiche ajoutée, média image/audio intégrés;
- **À CRÉER — lacune** : P981–P1000, toujours sans fiche détaillée repérée à ce stade.

Les index, catalogues, frises et pages de site ne font pas foi à eux seuls pour établir une fiche. Pour les lots anciens, les noms de fichiers ou les anciens journaux établissent le regroupement, mais un contrôle éditorial/structurel individualisé reste recommandé avant d’apposer une certification de qualité sur les 975 fiches antérieures. Médias manquants non évalués comme lacunes, conformément à l’instruction initiale de l’audit et aux décisions de la phase 10.

## Contrôles de liens
Un scan préalable des fichiers HTML a trouvé 149 références locales vers des fichiers HTML et aucune cible manquante. Les liens médias ne sont pas inclus dans ce résultat de contrôle. Pour le lot P976–P980, les cinq images et cinq audios sont maintenant enregistrés sous `preuves/images/` et `preuves/audio/`; le HTML du lot les référence relativement.
