---
title: "Tsk.RemainingWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le temps encore nécessaire pour terminer une tâche ou un ensemble de tâches"
type: docs
weight: 990
url: /fr/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

Le temps encore nécessaire pour terminer une tâche ou un ensemble de tâches.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


