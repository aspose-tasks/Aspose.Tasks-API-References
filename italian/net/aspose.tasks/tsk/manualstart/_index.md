---
title: "Tsk.ManualStart"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Definisce l'inizio programmato manualmente di un'attività"
type: docs
weight: 800
url: /it/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

Definisce l'inizio programmato manualmente di un'attività.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.ManualStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


