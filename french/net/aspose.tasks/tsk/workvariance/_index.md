---
title: "Tsk.WorkVariance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La différence entre le travail de référence d’une tâche et le travail actuellement programmé"
type: docs
weight: 1160
url: /fr/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

La différence entre le travail de référence d'une tâche et le travail actuellement planifié.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.WorkVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


