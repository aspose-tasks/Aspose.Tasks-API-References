---
title: "OutlineCode.ValueGuid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "OutlineCode propriété. Obtient ou définit le GUID de la valeur dans la liste de valeurs. Le ValueGuid correspond au FieldGuid dans la liste de valeurs"
type: docs
weight: 30
url: /fr/net/aspose.tasks/outlinecode/valueguid/
---
## OutlineCode.ValueGuid property

Obtient ou définit le GUID de la valeur dans la liste de valeurs. Le ValueGuid correspond au FieldGuid dans la liste de valeurs.

```csharp
public string ValueGuid { get; set; }
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


