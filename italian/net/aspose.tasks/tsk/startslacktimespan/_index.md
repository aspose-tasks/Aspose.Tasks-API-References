---
title: "Tsk.StartSlackTimeSpan"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La durata tra le date di Inizio Anticipato e Inizio Ritardato"
type: docs
weight: 1020
url: /it/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

La durata tra le date di Inizio Anticipato e Inizio Ritardato.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## Esempi

Mostra come leggere la proprietà Tsk.StartSlackTimeSpan. La proprietà è calcolata, quindi di solito non è necessario impostarla esplicitamente.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


