---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le temps pendant lequel une tâche peut être retardée sans retarder les tâches successeurs."
type: docs
weight: 450
url: /fr/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

Le temps pendant lequel une tâche peut être retardée sans retarder les tâches successeurs.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## Exemples

Montre comment lire la propriété Tsk.FreeSlackTimeSpan. La propriété est calculée, il n’est généralement pas nécessaire de la définir explicitement.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


