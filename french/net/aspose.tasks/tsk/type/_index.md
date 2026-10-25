---
title: "Tsk.Type"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Tsk field. Le type d'une tâche"
type: docs
weight: 1100
url: /fr/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

Le type d'une tâche.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.Type.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


