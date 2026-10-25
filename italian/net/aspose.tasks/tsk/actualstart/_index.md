---
title: "Tsk.ActualStart"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data e l'ora in cui un'attività è iniziata realmente"
type: docs
weight: 80
url: /it/net/aspose.tasks/tsk/actualstart/
---
## Tsk.ActualStart field

La data e l'ora in cui un'attività è effettivamente iniziata.

```csharp
public static readonly Key<DateTime, TaskKey> ActualStart;
```

## Esempi

Mostra che le date del progetto vengono reimpostate in modalità di valutazione.

```csharp
var project = new Project();

// crea nuove attività
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


