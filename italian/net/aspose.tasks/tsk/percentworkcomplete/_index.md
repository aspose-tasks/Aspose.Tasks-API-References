---
title: "Tsk.PercentWorkComplete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Lo stato attuale di un'attività espresso come percentuale del lavoro completato"
type: docs
weight: 890
url: /it/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

Lo stato attuale di un'attività espresso come percentuale del lavoro completato.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.PercentWorkComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


