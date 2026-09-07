---
title: "Tsk.IsExpanded"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se un'attività riepilogativa è espansa o meno nella visualizzazione GanttChart"
type: docs
weight: 590
url: /it/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

Determina se un'attività riepilogo è espansa o meno nella visualizzazione GanttChart.

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsExpanded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


