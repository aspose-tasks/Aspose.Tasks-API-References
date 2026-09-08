---
title: "Tsk.LevelAssignments"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk field. Bepaalt of de leveling-functie individuele toewijzingen kan vertragen en splitsen om overallocaties op te lossen"
type: docs
weight: 750
url: /nl/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

Bepaalt of de leveling-functie individuele toewijzingen kan vertragen en splitsen om overallocaties op te lossen.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.LevelAssignments te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


