---
title: "MPPSaveOptions.WriteViewData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà MPPSaveOptions. Ottiene o imposta un valore che indica se scrivere i dati della vista durante il salvataggio di un progetto in formato MPP. I dati della vista includono le collezioni Project.Views, Filters e Tables."
type: docs
weight: 80
url: /it/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

Ottiene o imposta un valore che indica se scrivere i dati della visualizzazione durante il salvataggio di un progetto in formato MPP. I dati della visualizzazione includono le collezioni Project.Views, Filters e Tables.

```csharp
public bool WriteViewData { get; set; }
```

## Esempi

Mostra come salvare il progetto in uno stream come file MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // crea opzioni di salvataggio
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // imposta un valore che indica se rimuovere le assegnazioni di risorse non valide durante il salvataggio in MPP
        RemoveInvalidAssignments = true
    };

    // salva MPP con opzioni
    project.Save(stream, options);
}
```

### Vedi anche

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


