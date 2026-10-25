---
title: "Tsk.IsNull"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si une tâche est une tâche nulle."
type: docs
weight: 640
url: /fr/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

Détermine si une tâche est une tâche nulle.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsNull.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


