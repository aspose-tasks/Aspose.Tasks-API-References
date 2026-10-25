---
title: "Tsk.ManualFinish"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Definisce la data di fine pianificata manualmente di un'attività"
type: docs
weight: 790
url: /it/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

Definisce il completamento programmato manualmente di un'attività.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.ManualFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


