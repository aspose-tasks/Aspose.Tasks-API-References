---
title: "Tsk.FinishVariance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le temps qui représente la différence entre la date de fin de base d’une tâche ou d’une affectation et sa date de fin actuelle"
type: docs
weight: 420
url: /fr/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

Le temps qui représente la différence entre la date de fin de référence d'une tâche ou d'une affectation et sa date de fin actuelle.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.FinishVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


