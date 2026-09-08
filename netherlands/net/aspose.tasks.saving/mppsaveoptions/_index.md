---
title: "Klasse MPPSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.MPPSaveOptions klasse. Stelt u in staat extra opties op te geven bij het opslaan van projectgegevens naar MPP"
type: docs
weight: 2050
url: /nl/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

Staat toe extra opties op te geven bij het opslaan van projectgegevens naar MPP.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | Initialiseert een nieuw exemplaar van de `MPPSaveOptions` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of bestaande VBA-macrogegevens moeten worden verwijderd bij het opslaan van een project in MPP-formaat. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | Haalt op of stelt een wachtwoord in dat wordt gebruikt om een resulterend MPP‑bestand te beveiligen. Momenteel wordt dit ondersteund voor MS Project 2010 en nieuwere formaten. Een null‑waarde geeft aan dat het projectbestand niet beveiligd is. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of ongeldige resource‑toewijzingen moeten worden verwijderd bij het opslaan naar MPP. MS Project maakt een lege resource‑toewijzing voor elke taak aan. Stel deze vlag in op true om ze bij het opslaan te verwijderen. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Haalt op of stelt het formaat in waarin het document wordt opgeslagen als dit opslaanopties‑object wordt gebruikt. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Haalt op of stelt de comparer in om taken te sorteren op het Gantt‑diagram en het Task‑Sheet‑diagram. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Haalt op of stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden gerenderd op Gantt‑, Task‑Sheet‑ en Task‑Usage‑diagrammen. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of filtergegevens moeten worden weggeschreven bij het opslaan van een project naar MPP-formaat. Filtergegevens omvatten de collecties Project.TaskFilters en Project.ResourceFilters. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of groepsgegevens moeten worden weggeschreven bij het opslaan van een project naar MPP-formaat. Groepsgegevens omvatten de collecties Project.TaskGroups en Project.ResourceGroups. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of bestaande VBA-macrogegevens in het MPP‑bestand moeten worden bijgewerkt. Momenteel wordt het schrijven van VbaModule.SourceCode ondersteund. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of weergavegegevens moeten worden weggeschreven bij het opslaan van een project naar MPP-formaat. Weergavegegevens omvatten de collecties Project.Views, Filters en Tables. |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


