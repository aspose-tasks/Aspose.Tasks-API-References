---
title: "Tsk.Deadline"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Una data obiettivo che indica quando un'attività deve essere completata"
type: docs
weight: 270
url: /it/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

Una data obiettivo che indica quando un'attività deve essere completata.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.Deadline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


