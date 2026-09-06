---
title: "Tsk.PreleveledStart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La date de début d’une tâche telle qu’elle était avant le nivellement des ressources"
type: docs
weight: 920
url: /fr/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

La date de début d’une tâche telle qu’elle était avant le nivellement des ressources.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.PreleveledStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


