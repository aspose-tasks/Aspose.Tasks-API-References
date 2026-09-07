---
title: "Tsk.Warning"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Rappresenta il flag che indica che l'attività ha discrepanze di programmazione"
type: docs
weight: 1120
url: /it/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

Rappresenta il flag che indica che il task ha discrepanze di programmazione.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## Esempi

Mostra come leggere un avviso di attività.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


