---
title: "OutlineCode.ValueGuid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "OutlineCode eigenschap. Haalt of stelt de GUID van de waarde in de waardelijst in. De ValueGuid komt overeen met de FieldGuid in de waardelijst"
type: docs
weight: 30
url: /nl/net/aspose.tasks/outlinecode/valueguid/
---
## OutlineCode.ValueGuid property

Haalt op of stelt de GUID van de waarde in de waardelijst in. De ValueGuid komt overeen met de FieldGuid in de waardelijst.

```csharp
public string ValueGuid { get; set; }
```

## Voorbeelden

Toont hoe de outline‑codes van een taak gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// outline‑codes lezen
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

### Zie ook

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


