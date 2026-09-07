---
title: "LevelingOptions.MessageHandler"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà LevelingOptions. Ottiene o imposta il callback del gestore dei messaggi che può essere usato per intercettare i messaggi di log prodotti da Aspose.Tasks durante il livellamento delle risorse"
type: docs
weight: 50
url: /it/net/aspose.tasks.leveling/levelingoptions/messagehandler/
---
## LevelingOptions.MessageHandler property

Ottiene o imposta il callback del gestore dei messaggi che può essere usato per intercettare i messaggi di log prodotti da Aspose.Tasks durante il livellamento delle risorse.

```csharp
public IMessageHandler MessageHandler { get; set; }
```

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

* interface [IMessageHandler](../../../aspose.tasks/imessagehandler/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


