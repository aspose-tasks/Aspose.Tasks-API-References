---
title: "Tsk.LateFinish"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La dernière date à laquelle une tâche peut se terminer sans retarder la fin du projet"
type: docs
weight: 730
url: /fr/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

La date la plus tardive à laquelle une tâche peut se terminer sans retarder la fin du projet.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.LateFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


