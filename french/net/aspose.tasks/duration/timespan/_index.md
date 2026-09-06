---
title: "Duration.TimeSpan"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Duration. Obtient l'instance TimeSpan de cet objet Duration. L'instance TimeSpan de cet objet Duration"
type: docs
weight: 40
url: /fr/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

Obtient l'instance `TimeSpan` de cet objet Duration. L'instance TimeSpan de cet objet Duration.

```csharp
public TimeSpan TimeSpan { get; }
```

## Exemples

Montre comment convertir une durée en TimeSpan.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// obtenir la durée de la tâche
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### Voir aussi

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


