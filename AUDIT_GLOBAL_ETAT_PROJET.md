# Audit global du projet « Prophéties »

**État : audit documentaire terminé sur le corpus local disponible — synthèse des lacunes et plan d’achèvement.**  
**Périmètre :** registres, fiches détaillées, index/catalogues, journaux de workflow et liens HTML locaux dans `propheties/preuves/`. Les médias absents ne sont pas traités comme des lacunes, conformément à la consigne de l’utilisateur.

## Résultat exécutif

Le projet est très avancé : le corpus comporte des registres allant jusqu’à **P1000**, un index qui annonce 1000 entrées, et des fiches HTML détaillées produites par lots, avec une fiche individuelle repérable pour P975. La principale lacune documentaire établie est la suite **P976–P1000** : ces 25 entrées figurent dans le registre complémentaire et les index, mais aucune fiche détaillée individuelle correspondante n’a été repérée dans les fichiers de fiches audités.

**Ne pas dire que P975 clôt le registre.** Cette conclusion antérieure était fausse : `23_REGISTRE_PROPHETIES_7.md` ajoute bien P976–P1000 et annonce P001–P1000. En revanche, une incohérence de version subsiste : `21_REGISTRE_PROPHETIES_6.md` se termine à P975, tandis que le registre complémentaire et l’index général portent le total à 1000.

## Réalisations constatées

- Plusieurs générations de registres couvrent le canon biblique de 66 livres retenu pour le projet. Les registres sont des versions successives et leurs plages/références se recoupent : ils ne doivent pas être additionnés naïvement.
- Les fiches anciennes sont regroupées par livre/catégorie dans des fichiers `FICHES8_…` et utilisent parfois des identifiants internes (par ex. GE001) plutôt que des ancres P. Les fiches récentes sont souvent regroupées par plages de six.
- Les fiches de Révélation repérées vont de P843–P848 à P969–P974, sans trou dans cette séquence de fichiers.
- Une fiche individuelle P975 existe : `FICHE_GEN_1_28_REVELATION_21_3-4_P975.html`.
- Les journaux phase 9 décrivent les vagues et les critères de rédaction (séparation lecture JW / faits indépendants / interprétations, limites, sources, workflow), mais le tracker présente des incohérences de numérotation et de statut.
- Vérification technique effectuée sur les références locales pointant vers des fichiers HTML : **149 cibles HTML, aucune cible manquante** dans les 211 pages HTML parcourues. Ce contrôle ne certifie pas les médias ni le fonctionnement de toutes les ancres internes.

## Lacunes réelles ou à résoudre

### 1. Fiches détaillées P976–P1000 — lacune confirmée (25)

Le registre complémentaire associe ces entrées aux livres suivants : P976–P980, Juges ; P981–P993, Marc ; P994, Colossiens ; P995–P1000, Jean. Ces identifiants apparaissent dans les outils de repérage/indexation, mais aucune fiche individuelle détaillée correspondante n’a été trouvée dans les fichiers de fiches. Une référence dans `INDEX_GENERAL.html`, le volume des 1000 ou une frise ne vaut pas fiche rédigée.

**Travail :** rédiger et intégrer 25 fiches, avec analyse, sources et limites selon le workflow. Ne pas générer les JPG/MP3 : leur absence est normale et l’utilisateur les possède.

### 2. Réconcilier les versions du registre et du tracker

- Le registre principal antérieur (partie 6) s’arrête à P975; le complément (partie 7) étend l’ensemble à P1000. Il faut expliciter qu’il s’agit d’un ajout/complément et aligner les en-têtes, pieds de page, compteurs et sources de génération.
- Dans `phase9/00_WORKFLOW_PHASE9.md`, des numéros de vague sont répétés ou non monotones (ex. la plage P933–P938 est signalée comme vague 57 après P927–P932 en vague 72; répétitions autour de la vague 72). Les chemins `../…` cités par le tracker doivent être validés depuis l’emplacement du tracker, pas supposés corrects.
- Refaire un tableau maître **ID → registre source → fichier/section de fiche → journal → état**. Le tracker seul ne constitue pas une preuve de présence ou d’achèvement.

### 3. Revue éditoriale, sources et complétude des dossiers

Le workflow revendique une méthode solide, mais un audit global de qualité fiche par fiche (dix rubriques, qualité/actualité des références, attribution des interprétations, examen des liens JW/WOL et des sources académiques) n’est pas certifié par le présent inventaire. Il reste à contrôler cette conformité et à corriger les écarts sans présenter une interprétation confessionnelle comme un fait historique. Garder le cadre canonique JW de 66 livres et attribuer explicitement à JW les affirmations qui lui sont propres.

Les recherches dans forums, YouTube et réseaux sociaux ne sont pas exhaustives à l’échelle du projet. Elles ne doivent pas être revendiquées comme telles; ces contenus, lorsqu’ils sont utilisés, relèvent de la réception/opinion et non de la preuve experte.

### 4. Contrôles techniques restant à automatiser

Le contrôle a vérifié les cibles locales HTML mais n’a pas certifié toutes les ancres internes, toutes les ressources non-HTML, ni le rendu/impression de chaque page. Faire un contrôle ciblé après intégration des fiches manquantes : ancres et navigation, chemins relatifs, validité HTML, index et compteur, affichage mobile/impression. Pour les liens médias, ne pas signaler une absence comme tâche de régénération; vérifier seulement les références et chemins si nécessaire.

## Hors périmètre des travaux restants

- **Aucune génération ou restauration de JPG/MP3.** L’utilisateur les conserve; leur absence actuelle résulte d’une suppression antérieure et est attendue.
- Ne pas recréer les fiches/médias des lots déjà terminés, notamment P867–P872, P879–P884, P885–P890 et P891–P896.
- Les illustrations restent des représentations, pas des preuves historiques; toute scène violente demeure non graphique.

## Ordre de priorité recommandé

1. Rédiger les fiches détaillées P976–P1000 en lots, puis les intégrer sans médias.
2. Corriger le tracker et ses chemins; consolider le registre à 1000 entrées en documentant la relation entre parties 6 et 7.
3. Reconstituer le tableau maître des 1000 IDs et vérifier chaque entrée contre une fiche réellement rédigée (pas seulement indexée).
4. Faire la revue éditoriale et les contrôles techniques approfondis, puis mettre à jour index, compteurs et statut final.

## Limites de cet audit

L’inventaire repose sur les fichiers présents dans le workspace et sur la structure observable des HTML, noms de fichiers et journaux. Les anciennes fiches n’emploient pas toutes le même balisage; un simple scan d’ancres P sous-estime leur couverture. Les conclusions de lacune ci-dessus ont donc été recoupées avec les fichiers de fiches, les journaux et les index, plutôt que déduites d’un tracker ou d’une recherche regex unique. Cet audit ne prétend pas certifier l’exactitude exégétique de chaque fiche ni l’exhaustivité du web social.
