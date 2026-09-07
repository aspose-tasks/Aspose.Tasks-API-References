---
title: "ResourceLeveler.LevelResources"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceLeveler. Livella le attività per le risorse specificate utilizzando le opzioni di livellamento specificate."
type: docs
weight: 30
url: /it/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

Livella le attività per le risorse specificate utilizzando le opzioni di livellamento specificate.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| progetto | Project | Progetto a cui applicare il livellamento delle risorse. |
| opzioni | LevelingOptions | Opzioni che specificano come livellare le risorse. |

### Valore di ritorno

Oggetto contenente i risultati del livellamento delle risorse.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | se il parametro options è nullo. |

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


