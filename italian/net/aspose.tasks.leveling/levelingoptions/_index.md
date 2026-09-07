---
title: "Classe LevelingOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Leveling.LevelingOptions. Consente di specificare i parametri del livellamento delle risorse"
type: docs
weight: 940
url: /it/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

Consente di specificare i parametri del livellamento delle risorse.

```csharp
public sealed class LevelingOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | Inizializza una nuova istanza della classe `LevelingOptions`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | Ottiene o imposta un token che può essere usato per annullare un'operazione di livellamento del progetto. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | Ottiene o imposta la data di fine del periodo di livellamento. Il valore predefinito è la data di conclusione del progetto. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | Ottiene l'ordine con cui l'algoritmo di livellamento ritarda le attività che hanno sovrallocazioni. Dopo aver determinato le attività che causano la sovrallocazione e quali attività possono essere ritardate, viene utilizzato l'ordine specificato per decidere quale attività ritardare per prima. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | Ottiene o imposta il callback del gestore dei messaggi che può essere usato per intercettare i messaggi di log prodotti da Aspose.Tasks durante il livellamento delle risorse. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Ottiene o imposta il livello dei messaggi di log emessi da Aspose.Tasks durante il livellamento delle risorse. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | Ottiene o imposta l'elenco delle risorse che saranno livellate. Se viene impostato null, tutte le risorse del progetto saranno livellate. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | Ottiene o imposta la data di inizio del periodo di livellamento. Il valore predefinito è la data di inizio del progetto. |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


