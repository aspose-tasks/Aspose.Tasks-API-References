---
title: "Tsk.RemainingDuration"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le temps nécessaire pour terminer la partie inachevée d’une tâche"
type: docs
weight: 960
url: /fr/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

Le temps nécessaire pour terminer la partie inachevée d’une tâche.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.RemainingDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


