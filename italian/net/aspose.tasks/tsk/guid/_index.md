---
title: "Tsk.Guid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. I codici di identificazione unici generati per un'attività"
type: docs
weight: 460
url: /it/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

I codici di identificazione unici generati per un'attività.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.Guid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


