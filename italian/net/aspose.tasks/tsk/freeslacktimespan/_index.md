---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il tempo in cui un'attività può essere ritardata senza ritardare alcuna attività successiva."
type: docs
weight: 450
url: /it/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

Il tempo in cui un'attività può essere ritardata senza ritardare le attività successive.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## Esempi

Mostra come leggere la proprietà Tsk.FreeSlackTimeSpan. La proprietà è calcolata, quindi di solito non è necessario impostarla esplicitamente.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


