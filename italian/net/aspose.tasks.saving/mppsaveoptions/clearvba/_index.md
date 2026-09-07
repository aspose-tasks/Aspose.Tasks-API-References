---
title: "MPPSaveOptions.ClearVba"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà MPPSaveOptions. Ottiene o imposta un valore che indica se rimuovere i dati delle macro VBA esistenti durante il salvataggio di un progetto in formato MPP."
type: docs
weight: 20
url: /it/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

Ottiene o imposta un valore che indica se rimuovere i dati delle macro VBA esistenti durante il salvataggio di un progetto in formato MPP.

```csharp
public bool ClearVba { get; set; }
```

## Esempi

Mostra come rimuovere le macro VBA dal file MPP.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### Vedi anche

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


