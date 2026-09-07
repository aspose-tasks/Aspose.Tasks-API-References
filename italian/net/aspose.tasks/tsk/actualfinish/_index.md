---
title: "Tsk.ActualFinish"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data in cui un'attività è stata completata"
type: docs
weight: 40
url: /it/net/aspose.tasks/tsk/actualfinish/
---
## Tsk.ActualFinish field

La data in cui un'attività è stata completata.

```csharp
public static readonly Key<DateTime, TaskKey> ActualFinish;
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


