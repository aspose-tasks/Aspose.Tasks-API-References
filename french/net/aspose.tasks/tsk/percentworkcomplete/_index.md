---
title: "Tsk.PercentWorkComplete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. L’état actuel d’une tâche exprimé en pourcentage du travail qui a été accompli"
type: docs
weight: 890
url: /fr/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

L’état actuel d’une tâche exprimé en pourcentage du travail qui a été accompli.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.PercentWorkComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


