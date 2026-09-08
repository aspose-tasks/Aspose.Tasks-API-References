---
title: "Project.DisplayOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projecteigenschap. Haalt een instantie van de ProjectDisplayOptions-klasse op"
type: docs
weight: 380
url: /nl/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

Haalt een instantie van de [`ProjectDisplayOptions`](../../projectdisplayoptions/) klasse op.

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## Voorbeelden

Toont hoe de weergaveopties van het project af te stemmen.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Stel een waarde in die aangeeft of waarschuwingen moeten worden weergegeven wanneer Project een mogelijk planningsconflict detecteert met een handmatig ingeplande taak.
// Deze optie is beschikbaar voor Project 2010 en later.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### Zie ook

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


