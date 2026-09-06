---
title: "Tsk.Stop"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La date qui représente la fin de la partie réelle d'une tâche."
type: docs
weight: 1060
url: /fr/net/aspose.tasks/tsk/stop/
---
## Tsk.Stop field

La date qui représente la fin de la partie réelle d'une tâche.

```csharp
public static readonly Key<DateTime, TaskKey> Stop;
```

## Exemples

Montre comment lire les dates d'arrêt/reprise d'une tâche.

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Vérifiez les dates d'arrêt et de reprise pour toutes les tâches.
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


