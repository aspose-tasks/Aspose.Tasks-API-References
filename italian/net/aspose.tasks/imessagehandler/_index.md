---
title: "Interfaccia IMessageHandler"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Interfaccia Aspose.Tasks.IMessageHandler. Rappresenta un callback dei risultati del livellamento delle risorse"
type: docs
weight: 880
url: /it/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

Rappresenta una callback per i risultati del livellamento delle risorse.

```csharp
public interface IMessageHandler
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks invoca questo metodo quando genera un messaggio. |

## Esempi

Mostra come livellare una risorsa specifica, personalizzare le opzioni di livellamento e esaminare i messaggi dell'algoritmo di livellamento.

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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


