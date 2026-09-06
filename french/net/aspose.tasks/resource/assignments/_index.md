---
title: "Resource.Assignments"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Resource. Obtient une collection d'affectations de ressources pour cet objet"
type: docs
weight: 120
url: /fr/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

Obtient une collection d'affectations de ressources pour cet objet.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Exemples

Montre comment lire les affectations d'une ressource.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

foreach (var resource in project.Resources)
{
    foreach (var assignment in resource.Assignments)
    {
        Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
        Console.WriteLine("Assignment's task name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
    }
}
```

### Voir aussi

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


