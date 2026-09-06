---
title: "Tsk.LevelAssignments"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si la fonction de nivellement peut retarder et diviser les affectations individuelles afin de résoudre les surallocations"
type: docs
weight: 750
url: /fr/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

Détermine si la fonction de nivellement peut retarder et diviser les affectations individuelles afin de résoudre les sur‑allocations.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.LevelAssignments.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


