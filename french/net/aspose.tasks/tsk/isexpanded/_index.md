---
title: "Tsk.IsExpanded"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si une tâche récapitulative est développée ou non dans la vue GanttChart"
type: docs
weight: 590
url: /fr/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

Détermine si une tâche récapitulative est développée ou non dans la vue GanttChart.

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsExpanded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


