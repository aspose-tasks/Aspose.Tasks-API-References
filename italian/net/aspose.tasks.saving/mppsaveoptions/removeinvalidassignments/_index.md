---
title: "MPPSaveOptions.RemoveInvalidAssignments"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà MPPSaveOptions. Ottiene o imposta un valore che indica se rimuovere le assegnazioni di risorse non valide durante il salvataggio in MPP. MS Project crea un'assegnazione di risorsa vuota per ogni attività. Impostare questo flag su true per rimuoverle al salvataggio."
type: docs
weight: 40
url: /it/net/aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/
---
## MPPSaveOptions.RemoveInvalidAssignments property

Ottiene o imposta un valore che indica se rimuovere le assegnazioni di risorse non valide durante il salvataggio in MPP. MS Project crea un'assegnazione di risorsa vuota per ogni attività. Imposta questo flag su true per rimuoverle al salvataggio.

```csharp
public bool RemoveInvalidAssignments { get; set; }
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


