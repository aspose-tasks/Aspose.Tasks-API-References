---
title: "Duration.ToString"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-methode. Geeft een tekenreeksrepresentatie van deze instantie terug"
type: docs
weight: 120
url: /nl/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

Retourneert een tekenreeksrepresentatie van deze instantie.

```csharp
public override string ToString()
```

### Retourwaarde

een tekenreeksrepresentatie van deze instantie.

## Voorbeelden

Toont hoe een duur naar een tekenreeks te converteren.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// haal de taakduur op
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### Zie ook

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


