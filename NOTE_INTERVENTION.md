# Note d'intervention — 6 novembre 2026

## Objectif et périmètre

Créer une landing page consultable pour le Drop 01 de HORS CHAMP à partir du brief fourni. Hypothèse retenue : le brief est une demande de réalisation du prototype. Aucun dépôt, ancienne version, photographie ou document DESIGN.md existant n'a été fourni.

## Sources consultées

Brief utilisateur, palette, architecture, descriptions de produits et YAML inclus dans le message. Aucun benchmark de marques n'a été consulté sur le web ; aucune recherche externe ou revendication de comparaison n'est présentée. Le travail ne passe pas par Google AI Studio.

## Actions réellement réalisées et choix

Création d'un site statique HTML/CSS/JavaScript autonome avec les neuf parties du brief. Illustrations SVG originales utilisées comme placeholders, identifiées comme études conceptuelles. Présentation craie/carbone, accent rouille dans le hero, vert signal dans l'accès anticipé. Fiches produit en fenêtres natives, menu mobile, accordéons et simulation du formulaire. Aucun envoi ou enregistrement d'email. Aucun prix, stock, compte ou paiement. Instagram et Contact ouvrent une information honnête au lieu de liens inventés.

Création de DESIGN.md et content.yaml ; ajout d'un générateur Python qui compile les principaux contenus du YAML dans le HTML. Les contenus secondaires et la structure se modifient dans le gabarit, comme précisé dans README.md. Le document de design décrit les variables réellement implémentées.

Fichiers créés : index.html, dist/index.html, DESIGN.md, content.yaml, build.py, requirements.txt, README.md et cette note. Dossier neuf ; aucun dépôt ou fichier préexistant modifié. Pas de publication, de modification des accès, de production, de message ou de dépense externe.

## Tests réellement exécutés

| Vérification | Résultat |
| --- | --- |
| Génération Python depuis content.yaml | Réussie |
| Syntaxe JavaScript, node --check | Réussie |
| Ancres internes | Toutes résolues |
| Identifiants HTML dans le document initial | Uniques |
| Structure principale | Un h1, quatre produits, un formulaire |
| Parité index.html et dist/index.html | Identiques |
| Recherche de fetch, XMLHttpRequest, localStorage, sessionStorage et URLs HTTP dans le HTML | Aucun appel ni stockage intégré trouvé |
| Rendu visuel Chrome sur écran large | Inspecté |
| Rendu mobile dans une iframe de 390 px (zone utile 375 px avec barre de défilement) | Inspecté ; largeur du document 375 px, sans débordement horizontal |
| Menu mobile puis lien Collection | Ouverture et repli après navigation confirmés |
| Fiche Field Hoodie sur écran large | Ouverture et CTA vers accès anticipé confirmés |
| Fiche Layer Shell sur mobile | Ouverture puis fermeture Échap confirmées, focus rendu à la carte |
| Accordéon matière sur mobile | Ouverture et contenu confirmés |
| Formulaire avec demo@example.org, écran large puis mobile | Message de simulation affiché ; champ réinitialisé |

Un essai d'ouverture des outils développeur a été refusé par la configuration du navigateur. La vérification responsive a été réalisée ensuite dans une iframe de test ; aucun contournement de cette restriction. Deux sélecteurs/lectures de test n'étaient pas supportés ou ne correspondaient pas au nom accessible ; les états ont ensuite été vérifiés par les contrôles visibles et une lecture DOM autorisée.

## Limites et prochaine action

Pas de test sur iPhone physique, Safari ou Firefox ; pas d'audit complet WCAG ou de mesure de performance. Le rendu typographique dépend des polices système. Le formulaire constitue une simulation, et les coordonnées, documents légaux, compte Instagram et caractéristiques définitives ne sont pas disponibles. Les études visuelles sont à remplacer par des images validées si la marque devient réelle.

Aucun blocage pour consulter la démonstration. Prochaine action proposée : revue du prototype et de la direction visuelle ; un déploiement ou une collecte réelle demandera une instruction explicite.

## Préparation GitHub — 6 novembre 2026

Objectif : créer un dépôt GitHub privé pour le projet et y pousser les sources livrées. Compte connecté vérifié : robindevoucoux1-cmyk. Fichiers existants retrouvés dans le dossier de travail.

Ajout de .gitignore pour exclure les environnements, secrets, métadonnées d'aperçu et page de contrôle mobile. Préparation d'un dépôt Git local sur main. Le site et son design n'ont pas été modifiés. Les tests fonctionnels ci-dessus concernent la version précédente, identique pour les fichiers du site ; ils n'ont pas été relancés pour cette préparation Git.

Blocage : le connecteur GitHub ne propose pas la création de dépôt ou l'envoi des sources ; gh n'est pas authentifié. Le navigateur connecté ne retrouve pas le contexte d'origine. Aucun dépôt distant, projet GitHub ou déploiement n'est annoncé comme créé. Prochaine action : rétablir l'accès au navigateur connecté pour créer le dépôt privé et y envoyer les sources.

## Dépôt HORSCHAMP — 6 novembre 2026

Le dépôt privé robindevoucoux1-cmyk/HORSCHAMP a été retrouvé via la liste des dépôts du compte connecté. Son état initial a été vérifié : aucun fichier et aucune branche. Les droits d'écriture sont confirmés. Le connecteur propose désormais les opérations d'écriture nécessaires.

Périmètre autorisé : déposer la landing page et sa documentation sur main dans ce dépôt neuf, sans déploiement. Les fichiers de prévisualisation, secrets et environnements sont exclus. Ajout de cette note ; aucun changement du code de la page. Aucun test fonctionnel relancé puisque le code livré est inchangé ; les tests réalisés sur la landing page sont consignés plus haut. La vérification distante porte sur les fichiers et les références Git après l'envoi.
