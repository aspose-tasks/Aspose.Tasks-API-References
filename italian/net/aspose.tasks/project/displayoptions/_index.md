---
title: "Project.DisplayOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà del progetto. Ottiene un'istanza della classe ProjectDisplayOptions"
type: docs
weight: 380
url: /it/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

Ottiene un'istanza della classe [`ProjectDisplayOptions`](../../projectdisplayoptions/).

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## Esempi

Mostra come ottimizzare le opzioni di visualizzazione del progetto.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Imposta un valore che indica se mostrare avvisi quando Project identifica un possibile conflitto di pianificazione con un'attività programmata manualmente.
// Questa opzione è disponibile per la versione Project 2010 e successive.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### Vedi anche

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


