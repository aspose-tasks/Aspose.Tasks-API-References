---
title: "Tsk.EarlyFinish"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La date la plus tôt à laquelle une tâche pourrait éventuellement se terminer, basée sur les dates de fin anticipée des tâches prédécesseurs et successeurs, d'autres contraintes et tout délai de nivellement"
type: docs
weight: 330
url: /fr/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

La date la plus tôt à laquelle une tâche pourrait éventuellement se terminer, basée sur les dates de fin anticipées des tâches prédécesseurs et successeurs, d'autres contraintes et tout retard de nivellement.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.EarlyFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


