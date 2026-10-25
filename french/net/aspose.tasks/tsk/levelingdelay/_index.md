---
title: "Tsk.LevelingDelay"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le temps pendant lequel une tâche doit être retardée par rapport à sa date de début anticipée en raison de l'équilibrage des ressources"
type: docs
weight: 770
url: /fr/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

Le temps pendant lequel une tâche doit être retardée par rapport à sa date de début au plus tôt en raison du nivellement des ressources.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.LevelingDelay.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


