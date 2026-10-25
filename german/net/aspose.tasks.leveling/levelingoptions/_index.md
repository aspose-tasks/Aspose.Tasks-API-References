---
title: "Klasse LevelingOptions"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.Leveling.LevelingOptions Klasse. Ermöglicht das Festlegen von Parametern für das Ressourcen-Leveling"
type: docs
weight: 940
url: /de/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

Ermöglicht das Festlegen von Parametern für das Ressourcen-Leveling.

```csharp
public sealed class LevelingOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | Initialisiert eine neue Instanz der `LevelingOptions` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | Ruft ein Token ab oder legt es fest, das zum Abbrechen einer Projekt-Leveling-Operation verwendet werden kann. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | Ruft das Enddatum des Leveling-Zeitraums ab oder legt es fest. Der Standardwert ist das Enddatum des Projekts. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | Ruft die Reihenfolge ab, in der der Leveling-Algorithmus Aufgaben mit Überbelegungen verzögert. Nachdem die Aufgaben, die die Überbelegung verursachen, und welche Aufgaben verzögert werden können, ermittelt wurden, wird die angegebene Reihenfolge verwendet, um zu bestimmen, welche Aufgabe zuerst verzögert werden soll. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | Ruft den Nachrichten-Handler-Callback ab oder legt ihn fest, der verwendet werden kann, um Protokollnachrichten von Aspose.Tasks während des Ressourcen-Levelings abzufangen. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Ruft das Protokoll-Level der von Aspose.Tasks während des Ressourcen-Levelings ausgegebenen Nachrichten ab oder legt es fest. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | Ruft die Liste der Ressourcen ab oder legt sie fest, die gelevelt werden sollen. Wenn null gesetzt ist, werden alle Projektressourcen gelevelt. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | Ruft das Startdatum des Leveling-Zeitraums ab oder legt es fest. Der Standardwert ist das Startdatum des Projekts. |

## Beispiele

Zeigt, wie man eine bestimmte Ressource ausgleicht, Ausgleichsoptionen anpasst und Nachrichten des Ausgleichsalgorithmus untersucht.

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

### Siehe auch

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


