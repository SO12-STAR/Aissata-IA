# Warehouse Control Tower

Application web front-end pour le projet final de Gestion Logistique d’Inventaires.

## Fichiers
- `control_tower_app.html` : application complète, autonome
- aucune installation serveur n’est nécessaire

## Exécution locale
1. Télécharger `control_tower_app.html`
2. Ouvrir le fichier dans un navigateur moderne
3. L’application charge automatiquement le dataset intégré

## Déploiement GitHub Pages
1. Créer un dépôt GitHub
2. Ajouter `control_tower_app.html`
3. Renommer le fichier en `index.html`
4. Activer GitHub Pages dans les paramètres du dépôt

## Fonctions incluses
- Module Inventaire BNMP
- Module UML As-Is / To-Be
- Module KPI / TRS
- Module Optimisation stock ABC/XYZ + EOQ
- Module Achats & Automatisation
- Module Transport & Répartition
- Module Monitoring / Exceptions
- Mini UAT
- Export CSV des exceptions, règles et audit log

## Remarques
- Les données inventaire et fournisseurs proviennent du fichier `warehouseops_dataset_350 (3).xlsx`.
- Les indicateurs transport sont simulés à partir de la pression d’achat et des zones fournisseurs, afin d’offrir une démonstration cohérente du module transport même sans fichier télémétrique séparé.
- Les modifications effectuées dans l’interface sont conservées dans le navigateur via `localStorage`.
- Pour réinitialiser la session, vider le stockage local du navigateur.

## JSON facultatif
L’application peut aussi charger un fichier JSON avec cette structure :
```json
{
  "items": [...],
  "suppliers": [...]
}
```
