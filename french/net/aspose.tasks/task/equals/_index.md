---
title: "Task.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Retourne une valeur indiquant si cette instance est égale à une tâche spécifiée"
type: docs
weight: 1330
url: /fr/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

Renvoie une valeur indiquant si cette instance est égale à une tâche spécifiée.

```csharp
public bool Equals(Task other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| autre | Tâche | La tâche spécifiée à comparer avec cette instance. |

### Valeur de retour

renvoie true si la tâche spécifiée et cette instance ont des identifiants uniques égaux.

## Exemples

Montre comment parcourir les affectations d'une tâche.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // afficher les affectations de la tâche
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | L'objet spécifié à comparer avec cette instance. |

### Valeur de retour

renvoie true si la tâche spécifiée et cette instance ont des identifiants uniques égaux.

## Exemples

Montre comment parcourir les affectations d'une tâche.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // afficher les affectations de la tâche
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Voir aussi

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


