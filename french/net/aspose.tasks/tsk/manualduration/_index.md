---
title: "Tsk.ManualDuration"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Définit la durée planifiée manuellement d'une tâche"
type: docs
weight: 780
url: /fr/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

Définit la durée planifiée manuellement d’une tâche.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.ManualDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


