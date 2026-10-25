---
title: "FilterCriteria"
second_title: "Aspose.Tasks pour Python via .NET Référence de l'API"
description: 
type: docs
weight: 350
url: /fr/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

Définit les critères que les tâches ou les ressources doivent satisfaire pour être affichés dans la vue MSP.

Le type FilterCriteria expose les membres suivants :
## Constructeurs
| Nom | Description |
| :- | :- |
| FilterCriteria() | Initialise une nouvelle instance de la classe FilterCriteria |
## Propriétés
| Nom | Description |
| :- | :- |
| opération | Obtient ou définit le critère établi avec FieldName, Test et Value qui se rapporte aux autres critères du filtre. |
| field | Obtient ou définit un [field](/tasks/python-net/aspose.tasks/filtercriteria/) à modifier. |
| test | Obtient ou définit le type de comparaison effectué entre FieldName et Value qui sert de critère de sélection pour le filtre.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | Obtient les valeurs d'objet à comparer avec la valeur du champ spécifié par FieldName. |
| criteria_rows | Obtient la liste des lignes enfants [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/).<br/>            Si le filtre contient plus d'une ligne de critère, l'effet d'un opérateur And est que les critères des deux lignes doivent être remplis pour que la tâche ou la ressource soit affichée en résultat de ce filtre.<br/>            L'effet d'un opérateur Or est que les critères de l'une ou l'autre ligne doivent être remplis. |
## Méthodes
| Nom | Description |
| :- | :- |
| is_field_value() | Obtient si la valeur à droite de FilterCriteria est une référence de champ, et non une valeur constante. |
| set_value_field(value) | Définit le champ dont la valeur sera comparée à la valeur du champ spécifié par FieldName. |

### Voir aussi

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

