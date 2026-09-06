---
title: "Tsk.PreleveledFinish"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La date de fin d'une tâche telle qu'elle était avant le nivellement des ressources."
type: docs
weight: 910
url: /fr/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

La date de fin d’une tâche telle qu’elle était avant le nivellement des ressources.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.PreleveledFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


