---
title: "Tsk.LevelingCanSplit"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Bepaalt of de resource-leveling functie splitsingen kan veroorzaken op het resterende werk van deze taak"
type: docs
weight: 760
url: /nl/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

Bepaalt of de resource-leveling-functie splitsingen kan veroorzaken in het resterende werk van deze taak.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.LevelingCanSplit te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


