---
title: "Tsk.StartVariance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le temps qui représente la différence entre la date de début de référence d’une tâche ou d’une affectation et sa date de début actuellement planifiée."
type: docs
weight: 1040
url: /fr/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

Le temps qui représente la différence entre la date de début de référence d'une tâche ou d'une affectation et sa date de début actuellement planifiée.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.StartVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


