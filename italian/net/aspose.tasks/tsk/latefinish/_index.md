---
title: "Tsk.LateFinish"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data più tarda in cui un'attività può terminare senza ritardare il completamento del progetto"
type: docs
weight: 730
url: /it/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

L'ultima data in cui un'attività può terminare senza ritardare la conclusione del progetto.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.LateFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


