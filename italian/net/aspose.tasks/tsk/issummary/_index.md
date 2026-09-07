---
title: "Tsk.IsSummary"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Tsk campo. Determina se un'attività è un'attività di riepilogo"
type: docs
weight: 720
url: /it/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

Determina se un'attività è un'attività riepilogo.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


