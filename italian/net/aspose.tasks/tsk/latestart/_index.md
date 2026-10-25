---
title: "Tsk.LateStart"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data più tarda in cui un'attività può iniziare senza ritardare il completamento del progetto"
type: docs
weight: 740
url: /it/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

L'ultima data in cui un'attività può iniziare senza ritardare la conclusione del progetto.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.LateStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


