# HORS CHAMP — Drop 01 / Outside System

Landing page de démonstration, autonome, sans backend ni dépendance de réseau à l'ouverture.

## Ouvrir

Double-cliquer sur `index.html`. Tout est intégré : styles, scripts et illustrations SVG. Aucun compte, serveur ou installation nécessaire pour consulter la page.

## Modifier les contenus

1. Modifier `content.yaml` : marque, promesse, nom et date du drop, CTA, manifeste, quatre produits, accès anticipé.
2. Avec Python 3 et PyYAML installé : `python3 build.py`.
3. Rouvrir `index.html` ou actualiser la page. `dist/index.html` est également régénéré.

Pour installer la seule dépendance de génération dans un environnement dédié :

```sh
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python3 build.py
```

Le script reste optionnel pour consulter le site ; le HTML peut aussi être édité directement. Une modification manuelle du HTML sera écrasée à la prochaine génération.

`DESIGN.md` décrit les décisions visuelles. Pour changer le design, modifier les variables et règles CSS du gabarit dans `build.py`, puis reconstruire.

Les textes éditoriaux complémentaires du lookbook, des accordéons et des fenêtres d'information se modifient dans le gabarit `build.py`. La structure est conçue pour les quatre pièces du brief. Les liens internes des CTA et du pied de page sont fixes ; les champs `href`, `territory`, `footer` et `backend_required` du YAML documentent le brief et ne constituent pas un CMS ou une configuration fonctionnelle.

## Formulaire

L'email est vérifié par le navigateur mais n'est pas stocké ni envoyé. Après soumission, le champ est effacé et un message annonce une simulation. Aucun service mail ou base de données n'est connecté.

## Livraison

- `index.html` : version autonome à ouvrir.
- `dist/index.html` : même version, préparée pour un hébergement statique futur.
- `content.yaml` : contenu éditorial modifiable.
- `DESIGN.md` : direction artistique.
- `build.py` et `requirements.txt` : génération facultative.
- `NOTE_INTERVENTION.md` : périmètre, vérifications et limites.

Aucune publication ni mise en production n'a été réalisée.
