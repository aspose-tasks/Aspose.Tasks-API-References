---
title: "Tsk.EarlyStart"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data più precoce in cui un'attività può iniziare, basata sulle date di inizio anticipate delle attività predecessore e successore e su altre restrizioni."
type: docs
weight: 340
url: /it/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

La data più precoce in cui un'attività potrebbe iniziare, basata sulle date di inizio anticipate delle attività predecessore e successore e altri vincoli.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.EarlyStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


