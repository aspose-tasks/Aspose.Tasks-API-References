---
title: "Klasse LevelingOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Leveling.LevelingOptions klasse. Stelt u in staat parameters van resource‑nivellering op te geven"
type: docs
weight: 940
url: /nl/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

Staat toe parameters van resource-leveling op te geven.

```csharp
public sealed class LevelingOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | Initialiseert een nieuw exemplaar van de `LevelingOptions` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | Haalt op of stelt een token in dat kan worden gebruikt om een projectnivelleringsbewerking te annuleren. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | Haalt op of stelt de einddatum van de nivelleringsperiode in. De standaardwaarde is de einddatum van het project. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | Haalt de volgorde op waarin het nivelleringsalgoritme taken met overallocaties vertraagt. Na bepaling van de taken die de overallocatie veroorzaken en welke taken kunnen worden vertraagd, wordt de opgegeven volgorde gebruikt om te bepalen welke taak eerst moet worden vertraagd. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | Haalt op of stelt de callback voor berichtafhandeling in die kan worden gebruikt om logberichten die door Aspose.Tasks tijdens resource‑nivellering worden geproduceerd, af te vangen. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Haalt op of stelt het niveau van logberichten in dat door Aspose.Tasks tijdens resource‑nivellering wordt uitgegeven. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | Haalt op of stelt de lijst van resources in die genivelleerd zullen worden. Als null wordt ingesteld, worden alle projectresources genivelleerd. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | Haalt op of stelt de startdatum van de nivelleringsperiode in. De standaardwaarde is de startdatum van het project. |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


