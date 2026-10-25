---
title: "Tsk.Deadline"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Une date cible indiquant quand une tâche doit être terminée"
type: docs
weight: 270
url: /fr/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

Une date cible indiquant quand une tâche doit être terminée.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.Deadline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


