---
title: "Task.Clone"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Taakmethode. Maakt een volledige kopie van een taak zonder subtaken"
type: docs
weight: 1310
url: /nl/net/aspose.tasks/task/clone/
---
## Task.Clone method

Maakt een volledige kopie van een taak zonder subtaken.

```csharp
public object Clone()
```

### Retourwaarde

Kopie van een taak gemaakt.

## Voorbeelden

Toont hoe een taak te klonen.

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


