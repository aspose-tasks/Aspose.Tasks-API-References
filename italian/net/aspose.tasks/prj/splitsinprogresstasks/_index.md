---
title: "Prj.SplitsInProgressTasks"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se le attività in corso possono essere suddivise"
type: docs
weight: 650
url: /it/net/aspose.tasks/prj/splitsinprogresstasks/
---
## Prj.SplitsInProgressTasks field

Determina se le attività in corso possono essere suddivise.

```csharp
public static readonly Key<NullableBool, PrjKey> SplitsInProgressTasks;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.SplitsInProgressTasks.

```csharp
var project = new Project();

project.Set(Prj.SplitsInProgressTasks, true);

Console.WriteLine("Splits In Progress Tasks: " + project.Get(Prj.SplitsInProgressTasks));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


