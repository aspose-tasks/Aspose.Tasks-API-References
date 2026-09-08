---
title: "MPPSaveOptions.WriteViewData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MPPSaveOptions‑eigenschap. Haalt een waarde op of stelt deze in die aangeeft of weergavegegevens moeten worden weggeschreven bij het opslaan van een project naar MPP‑formaat. Weergavegegevens omvatten de collecties Project.Views Filters en Tables."
type: docs
weight: 80
url: /nl/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

Haalt op of stelt een waarde in die aangeeft of weergavegegevens moeten worden weggeschreven bij het opslaan van een project naar MPP-formaat. Weergavegegevens omvatten de collecties Project.Views, Filters en Tables.

```csharp
public bool WriteViewData { get; set; }
```

## Voorbeelden

Toont hoe een project kan worden opgeslagen in een stream als een MPP‑bestand.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // maak opslagopties
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // stelt een waarde in die aangeeft of ongeldige resource‑toewijzingen moeten worden verwijderd bij het opslaan naar MPP
        RemoveInvalidAssignments = true
    };

    // sla MPP op met opties
    project.Save(stream, options);
}
```

### Zie ook

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


