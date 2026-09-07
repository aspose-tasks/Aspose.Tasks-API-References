---
title: "LevelingOptions.MessageLevel"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà LevelingOptions. Ottiene o imposta il livello dei messaggi di log generati da Aspose.Tasks durante il livellamento delle risorse"
type: docs
weight: 60
url: /it/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Ottiene o imposta il livello dei messaggi di log emessi da Aspose.Tasks durante il livellamento delle risorse.

```csharp
public MessageLevel MessageLevel { get; set; }
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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


