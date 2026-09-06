---
title: "Tsk.IsSummary"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si une tâche est une tâche récapitulative"
type: docs
weight: 720
url: /fr/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

Détermine si une tâche est une tâche récapitulative.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


