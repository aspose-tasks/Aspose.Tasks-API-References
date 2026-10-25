---
title: "Schnittstelle IMessageHandler"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.IMessageHandler Schnittstelle. Stellt einen Rückruf für die Ergebnisse der Ressourcen‑Ausgleichung dar"
type: docs
weight: 880
url: /de/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

Stellt einen Rückruf für die Ergebnisse der Ressourcen‑Ausgleichung dar.

```csharp
public interface IMessageHandler
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks ruft diese Methode auf, wenn eine Nachricht ausgegeben wird. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


