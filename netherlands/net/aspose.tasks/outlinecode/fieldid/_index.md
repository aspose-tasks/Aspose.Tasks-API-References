---
title: "OutlineCode.FieldId"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "OutlineCode eigenschap. Haalt of stelt de numerieke waarde van het aangepaste project‑Id‑veld in"
type: docs
weight: 20
url: /nl/net/aspose.tasks/outlinecode/fieldid/
---
## OutlineCode.FieldId property

Haalt op of stelt de numerieke waarde van het aangepaste veld project Id in.

```csharp
public string FieldId { get; set; }
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


