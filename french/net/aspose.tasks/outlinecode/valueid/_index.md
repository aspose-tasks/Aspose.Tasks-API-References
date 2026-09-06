---
title: "OutlineCode.ValueId"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "OutlineCode propriété. Obtient ou définit l'Id dans la liste de valeurs associé à la définition dans la collection de codes de plan"
type: docs
weight: 40
url: /fr/net/aspose.tasks/outlinecode/valueid/
---
## OutlineCode.ValueId property

Obtient ou définit l'Id dans la liste de valeurs associé à la définition dans la collection de codes de plan.

```csharp
public int ValueId { get; set; }
```

## Exemples

Montre comment lire les codes de plan d'une tâche.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// lire les codes de plan
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### Voir aussi

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


