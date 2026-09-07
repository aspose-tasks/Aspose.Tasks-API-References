---
title: "Tsk.IsMarked"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Indica se un'attività è contrassegnata per ulteriori azioni o per qualche tipo di identificazione"
type: docs
weight: 620
url: /it/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

Mostra se un'attività è contrassegnata per ulteriori azioni o per qualche tipo di identificazione.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## Osservazioni

Si applica solo al formato file mpp.

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsMarked.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


