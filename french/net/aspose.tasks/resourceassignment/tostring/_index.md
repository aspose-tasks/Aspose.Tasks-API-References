---
title: "ResourceAssignment.ToString"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceAssignment. Retourne une représentation sous forme de chaîne courte de l'instance de la classe ResourceAssignment. Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer"
type: docs
weight: 790
url: /fr/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

Retourne une représentation sous forme de chaîne courte de l'instance de la classe [`ResourceAssignment`](../). Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer.

```csharp
public override string ToString()
```

### Valeur de retour

chaîne courte qui représente l'objet d'affectation.

## Exemples

Montre comment afficher les informations d'affectation courantes.

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

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


