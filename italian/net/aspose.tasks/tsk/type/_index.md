---
title: "Tsk.Type"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il tipo di un'attività"
type: docs
weight: 1100
url: /it/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

Il tipo di un'attività.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.Type.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


