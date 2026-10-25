---
title: "MPPSaveOptions.ClearVba"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MPPSaveOptions‑eigenschap. Haalt een waarde op of stelt deze in die aangeeft of bestaande VBA‑macro‑gegevens moeten worden verwijderd bij het opslaan van een project naar MPP‑formaat."
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

Haalt op of stelt een waarde in die aangeeft of bestaande VBA-macrogegevens moeten worden verwijderd bij het opslaan van een project in MPP-formaat.

```csharp
public bool ClearVba { get; set; }
```

## Voorbeelden

Toont hoe u VBA‑macro's uit een MPP‑bestand kunt verwijderen.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### Zie ook

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


