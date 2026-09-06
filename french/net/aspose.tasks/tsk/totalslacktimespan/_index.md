---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le temps pendant lequel la date de fin d’une tâche peut être retardée sans retarder la date de fin du projet."
type: docs
weight: 1090
url: /fr/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

Le temps pendant lequel la date de fin d'une tâche peut être retardée sans retarder la date de fin du projet.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## Exemples

Montre comment lire la propriété Tsk.TotalSlackTimeSpan. La propriété est calculée, il n’est généralement pas nécessaire de la définir explicitement.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


