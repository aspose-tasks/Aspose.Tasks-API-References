---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La durée entre les dates de fin anticipée et de fin tardive"
type: docs
weight: 400
url: /fr/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

La durée entre les dates de fin anticipée et de fin tardive.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## Exemples

Montre comment lire la propriété Tsk.FinishSlackTimeSpan. La propriété est calculée, il n'est généralement pas nécessaire de la définir explicitement.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


