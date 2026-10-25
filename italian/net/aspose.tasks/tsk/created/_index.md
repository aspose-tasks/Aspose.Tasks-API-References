---
title: "Tsk.Created"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data in cui è stata creata un'attività"
type: docs
weight: 250
url: /it/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

La data in cui è stata creata un'attività.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.Created.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


