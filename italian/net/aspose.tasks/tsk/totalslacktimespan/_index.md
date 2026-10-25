---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il tempo in cui la data di fine di un'attività può essere ritardata senza ritardare la data di fine del progetto."
type: docs
weight: 1090
url: /it/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

Il tempo in cui la data di fine di un'attività può essere ritardata senza ritardare la data di fine del progetto.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## Esempi

Mostra come leggere la proprietà Tsk.TotalSlackTimeSpan. La proprietà è calcolata, quindi di solito non è necessario impostarla esplicitamente.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


