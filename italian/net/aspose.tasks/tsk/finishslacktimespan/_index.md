---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La durata tra le date di Fine Anticipata e Fine Ritardata"
type: docs
weight: 400
url: /it/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

La durata tra le date di fine anticipata e fine tardiva.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## Esempi

Mostra come leggere la proprietà Tsk.FinishSlackTimeSpan. La proprietà è calcolata, quindi di solito non è necessario impostarla esplicitamente.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


