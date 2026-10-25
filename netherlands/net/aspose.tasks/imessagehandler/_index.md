---
title: "Interface IMessageHandler"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.IMessageHandler interface. Vertegenwoordigt een callback voor de resultaten van resource leveling"
type: docs
weight: 880
url: /nl/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

Stelt een callback voor die de resultaten van resource leveling levert.

```csharp
public interface IMessageHandler
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks roept deze methode aan wanneer een bericht wordt uitgegeven. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


