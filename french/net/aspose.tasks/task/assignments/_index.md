---
title: "Task.Assignments"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient une collection d'affectations de ressources pour cet objet"
type: docs
weight: 120
url: /fr/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

Obtient une collection d'affectations de ressources pour cet objet.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

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

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


