---
title: "Tsk.IsSubproject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si une tâche est un projet inséré"
type: docs
weight: 700
url: /fr/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

Détermine si une tâche est un projet inséré.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsSubproject.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


