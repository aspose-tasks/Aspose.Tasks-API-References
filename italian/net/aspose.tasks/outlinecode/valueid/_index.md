---
title: "OutlineCode.ValueId"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà OutlineCode. Ottiene o imposta l'Id nella lista dei valori associato alla definizione nella collezione di outline code"
type: docs
weight: 40
url: /it/net/aspose.tasks/outlinecode/valueid/
---
## OutlineCode.ValueId property

Ottiene o imposta l'Id nella lista dei valori associato alla definizione nella collezione di codici di outline.

```csharp
public int ValueId { get; set; }
```

## Esempi

Mostra come leggere i codici di outline delle attività.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// leggi i codici di outline
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

### Vedi anche

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


