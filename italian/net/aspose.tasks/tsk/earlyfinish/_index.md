---
title: "Tsk.EarlyFinish"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data più precoce in cui un'attività potrebbe terminare, basata sulle date di fine anticipata delle attività predecessore e successore, altri vincoli e eventuali ritardi di livellamento"
type: docs
weight: 330
url: /it/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

La data più precoce in cui un'attività potrebbe terminare, basata sulle date di fine anticipate delle attività predecessore e successore, altri vincoli e eventuali ritardi di livellamento.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.EarlyFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


