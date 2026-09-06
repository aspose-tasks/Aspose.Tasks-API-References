---
title: "Tsk.DurationVariance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La différence entre la durée de référence d’une tâche et l’estimation actuelle de la durée totale d’une tâche."
type: docs
weight: 320
url: /fr/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

La différence entre la durée de référence d'une tâche et la durée totale (estimation actuelle) d'une tâche.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.DurationVariance.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


