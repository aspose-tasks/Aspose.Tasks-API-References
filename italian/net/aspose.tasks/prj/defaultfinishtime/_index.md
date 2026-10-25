---
title: "Prj.DefaultFinishTime"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il tempo di fine predefinito per le nuove attività"
type: docs
weight: 230
url: /it/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

L'ora di fine predefinita delle nuove attività.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.DefaultFinishTime.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


