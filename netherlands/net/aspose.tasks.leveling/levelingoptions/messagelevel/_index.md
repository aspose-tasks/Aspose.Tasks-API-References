---
title: "LevelingOptions.MessageLevel"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "LevelingOptions eigenschap. Haalt op of stelt het niveau van logberichten in die door Aspose.Tasks worden uitgegeven tijdens resource-leveling"
type: docs
weight: 60
url: /nl/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Haalt op of stelt het niveau van logberichten in dat door Aspose.Tasks tijdens resource‑nivellering wordt uitgegeven.

```csharp
public MessageLevel MessageLevel { get; set; }
```

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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


