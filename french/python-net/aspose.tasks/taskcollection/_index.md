---
title: "TaskCollection"
second_title: "Aspose.Tasks pour Python via .NET Référence de l'API"
description: 
type: docs
weight: 1140
url: /fr/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Représente une collection d'objets [Task](/tasks/python-net/aspose.tasks/task/).

Le type TaskCollection expose les membres suivants :
## Propriétés
| Nom | Description |
| :- | :- |
| parent_project | Obtient le projet parent de l'objet TaskCollection. |
## Méthodes
| Nom | Description |
| :- | :- |
| add() | Ajoutez la tâche spécifiée à l'instance de la classe [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/).<br/>            Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (Cela replanifiera toutes les tâches du projet (dates de début/fin, définit les dates anticipées/tardives) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les identifiants et les niveaux de hiérarchie).<br/>            Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'identifiant de la tâche, le niveau de hiérarchie et les numéros de hiérarchie automatiquement.<br/>            Si ParentProject.CalculationMode est Automatic, la méthode replanifie automatiquement toutes les tâches du projet<br/>            (dates de début/fin, définit les dates anticipées/tardives, calcule les marges, le travail et les champs de coût, recalculera les identifiants et les niveaux de hiérarchie). |
| add(task_name) | Ajoute une nouvelle tâche à la collection des tâches enfants. |
| add(task_name, before_task_id) |  |
| add(parameters) | Insère une nouvelle tâche avant une tâche avec l'identifiant spécifié et au même niveau de hiérarchie. |
| to_list() | Convertit l'objet TaskCollection en une liste d'objets [Task](/tasks/python-net/aspose.tasks/task/). |
| get_by_uid(uid) | Renvoie une tâche avec l'Uid spécifié dont l'ancêtre est la tâche parent de cette collection. |
| get_by_id(id) | Renvoie une tâche avec l'Id spécifié dont l'ancêtre est la tâche parent de cette collection. |

### Voir aussi

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

