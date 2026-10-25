---
title: "Méthode Aspose::Tasks::Task::MoveToSibling"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks pour C++"
description: "Déplace la tâche actuelle au même niveau de contour avant la tâche spécifiée."
type: docs
weight: 1370
url: /fr/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

Déplace la tâche actuelle au même niveau de plan (Outline Level) avant la tâche spécifiée. Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (cela replanifiera toutes les tâches du projet (dates de début/fin, définit les dates au plus tôt/au plus tard) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les niveaux de plan). Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'ID de la tâche, le niveau de plan et les numéros de plan automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifie automatiquement toutes les tâches du projet (dates de début/fin, définit les dates au plus tôt/au plus tard, calcule les marges, le travail et les champs de coût, recalculera les IDs et les niveaux de plan).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| Paramètre | Description |
| --- | --- |
| beforeTask | Tâche avant laquelle la tâche actuelle sera insérée. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

Déplace la tâche actuelle au même niveau de contour avant une tâche avec l'Id spécifié. Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (cela replanifiera toutes les tâches du projet (dates de début/fin, définit les dates anticipées/retardées) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les niveaux de contour). Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'identifiant de la tâche, le niveau de contour et les numéros de contour automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifie automatiquement toutes les tâches du projet (dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût, recalcul les identifiants et les niveaux de contour).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| Paramètre | Description |
| --- | --- |
| beforeTaskId | Id ( Tsk::Id ) d'une tâche avant laquelle la tâche actuelle sera insérée. |

