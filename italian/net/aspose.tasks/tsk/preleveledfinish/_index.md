---
title: "Tsk.PreleveledFinish"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data di fine di un'attività così com'era prima che fosse eseguito il livellamento delle risorse"
type: docs
weight: 910
url: /it/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

La data di completamento di un'attività com'era prima che fosse effettuato il livellamento delle risorse.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.PreleveledFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


