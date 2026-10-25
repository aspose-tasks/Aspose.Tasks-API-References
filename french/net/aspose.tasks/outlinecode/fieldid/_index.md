---
title: "OutlineCode.FieldId"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "OutlineCode propriété. Obtient ou définit la valeur numérique du champ personnalisé Id du projet"
type: docs
weight: 20
url: /fr/net/aspose.tasks/outlinecode/fieldid/
---
## OutlineCode.FieldId property

Obtient ou définit la valeur numérique du champ personnalisé Id du projet.

```csharp
public string FieldId { get; set; }
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


