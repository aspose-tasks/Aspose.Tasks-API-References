---
title: "Task.MoveToSibling"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Déplace la tâche actuelle au même niveau de planification avant la tâche spécifiée. Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate après avoir utilisé cette méthode. Elle replanifiera toutes les dates de début/fin des tâches du projet, définira les dates au plus tôt/au plus tard et calculera les champs dépendants tels que les marges, le travail et les champs de coût ainsi que les niveaux de planification. Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'ID de la tâche, le niveau de planification et les numéros de planification automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifie automatiquement toutes les tâches du projet, dates de début/fin, définit les dates au plus tôt/au plus tard, calcule les marges, le travail et les champs de coût, et recalculera les ID et les niveaux de planification."
type: docs
weight: 1370
url: /fr/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Déplace la tâche actuelle au même niveau d'outline avant la tâche spécifiée. Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (cela replanifiera toutes les tâches du projet (dates de début/fin, définit les dates anticipées/retardées) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les niveaux d'outline). Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'Id de la tâche, le niveau d'outline et les numéros d'outline automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifie automatiquement toutes les tâches du projet (dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût, recalcul les Id et les niveaux d'outline).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| beforeTask | Tâche | Tâche avant laquelle la tâche actuelle sera insérée. |

## Exemples

Montre comment déplacer la tâche sous le même parent.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Déplacer les tâches avec l'ID 5 avant la tâche avec l'ID 3
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// OU
// Déplacer la tâche à la fin de la collection
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Déplace la tâche actuelle au même niveau d'outline avant une tâche avec l'Id spécifié. Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (cela replanifiera toutes les tâches du projet (dates de début/fin, définit les dates anticipées/retardées) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les niveaux d'outline). Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'Id de la tâche, le niveau d'outline et les numéros d'outline automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifie automatiquement toutes les tâches du projet (dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût, recalcul les Id et les niveaux d'outline).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| beforeTaskId | Int32 | Id ([`Id`](../../tsk/id/)) d'une tâche avant laquelle la tâche actuelle sera insérée. |

## Exemples

Montre comment déplacer la tâche sous le même parent en utilisant l'Id de la tâche.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Déplacer les tâches avec l'ID 5 avant la tâche avec l'ID 3
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// OU
// Déplacer la tâche à la fin de la collection
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


