---
title: "ResourceLeveler.LevelResources"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceLeveler method. Voert leveling uit op taken voor de opgegeven resources met de opgegeven leveling-opties."
type: docs
weight: 30
url: /nl/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

Nivelleert taken voor de opgegeven resources met de opgegeven nivelleringsopties.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | Project om resource-leveling toe te passen. |
| opties | LevelingOptions | Opties die aangeven hoe resources te levelen. |

### Retourwaarde

Object dat de resultaten van resource-leveling bevat.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentNullException | als parameter options null is. |

## Voorbeelden

Toont hoe een specifieke resource te nivelleren, nivelleringopties aan te passen en berichten van het nivelleringalgoritme te bekijken.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### Zie ook

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


