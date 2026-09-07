---
title: "Tsk.PreleveledStart"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Tsk campo. La data di inizio di un'attività così com'era prima che fosse effettuato il livellamento delle risorse"
type: docs
weight: 920
url: /it/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

La data di inizio di un'attività com'era prima che fosse effettuato il livellamento delle risorse.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.PreleveledStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


