---
title: "MPPSaveOptions.RemoveInvalidAssignments"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MPPSaveOptions‑eigenschap. Haalt een waarde op of stelt deze in die aangeeft of ongeldige resource‑toewijzingen moeten worden verwijderd bij het opslaan naar MPP. MS Project maakt voor elke taak een lege resource‑toewijzing aan. Stel deze vlag in op true om ze bij het opslaan te verwijderen."
type: docs
weight: 40
url: /nl/net/aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/
---
## MPPSaveOptions.RemoveInvalidAssignments property

Haalt op of stelt een waarde in die aangeeft of ongeldige resource‑toewijzingen moeten worden verwijderd bij het opslaan naar MPP. MS Project maakt een lege resource‑toewijzing voor elke taak aan. Stel deze vlag in op true om ze bij het opslaan te verwijderen.

```csharp
public bool RemoveInvalidAssignments { get; set; }
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


