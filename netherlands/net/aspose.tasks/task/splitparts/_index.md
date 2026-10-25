---
title: "Task.SplitParts"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task eigenschap. Haalt een SplitPart-collectie op die de delen van een taak weergeeft"
type: docs
weight: 1110
url: /nl/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

Haalt een SplitPart-collectie op die de delen van een taak weergeeft.

```csharp
public SplitPartCollection SplitParts { get; }
```

## Voorbeelden

Toont hoe de gesplitste delen van een taak worden weergegeven.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// Taak openen
var task = project.RootTask.Children.GetById(4);

// Gesplitste delen van een taak weergeven
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### Zie ook

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


