---
title: "Tsk.ManualFinish"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Définit la fin planifiée manuellement d'une tâche"
type: docs
weight: 790
url: /fr/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

Définit la date de fin planifiée manuellement d’une tâche.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.ManualFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


