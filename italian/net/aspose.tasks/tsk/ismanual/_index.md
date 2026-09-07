---
title: "Tsk.IsManual"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Tsk campo. Determina se un'attività è pianificata manualmente"
type: docs
weight: 610
url: /it/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

Determina se un'attività è pianificata manualmente.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsManual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


