---
title: "Tsk.IsManual"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si une tâche est planifiée manuellement"
type: docs
weight: 610
url: /fr/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

Détermine si une tâche est planifiée manuellement.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsManual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


