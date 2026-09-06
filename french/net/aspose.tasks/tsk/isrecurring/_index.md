---
title: "Tsk.IsRecurring"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si une tâche fait partie d’une série de tâches récurrentes"
type: docs
weight: 670
url: /fr/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

Détermine si une tâche fait partie d’une série de tâches récurrentes.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsRecurring.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


