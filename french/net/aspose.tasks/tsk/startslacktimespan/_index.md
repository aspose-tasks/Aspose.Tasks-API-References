---
title: "Tsk.StartSlackTimeSpan"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La durée entre les dates de début précoce et de début tardif"
type: docs
weight: 1020
url: /fr/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

La durée entre les dates de début précoce et de début tardif.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## Exemples

Montre comment lire la propriété Tsk.StartSlackTimeSpan. La propriété est calculée, il n'est généralement pas nécessaire de la définir explicitement.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


