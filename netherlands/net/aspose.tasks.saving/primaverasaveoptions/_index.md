---
title: "Class PrimaveraSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.PrimaveraSaveOptions class. Stelt u in staat extra opties op te geven bij het opslaan van een project naar het Primavera XER-formaat"
type: docs
weight: 2150
url: /nl/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

Staat toe extra opties op te geven bij het opslaan van een project naar het Primavera XER‑formaat.

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | Initialiseert een nieuw exemplaar van de `PrimaveraSaveOptions` class. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | Haalt op of stelt de increment in die wordt gebruikt bij het hernummeren van activiteit-ID's. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | Haalt op of stelt het voorvoegsel in dat wordt gebruikt bij het hernummeren van activiteit-ID's. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | Haalt op of stelt het achtervoegsel in dat wordt gebruikt bij het hernummeren van activiteit-ID's. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of activiteit-ID's moeten worden hergenummerd. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Haalt op of stelt het formaat in waarin het document wordt opgeslagen als dit opslaanopties‑object wordt gebruikt. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Haalt op of stelt de comparer in om taken te sorteren op het Gantt‑diagram en het Task‑Sheet‑diagram. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Haalt op of stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden gerenderd op Gantt‑, Task‑Sheet‑ en Task‑Usage‑diagrammen. |

## Voorbeelden

Toont hoe te werken met &lt;see cref=\"Aspose.Tasks.Saving.PrimaveraSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// maak Primavera opslaanopties en stem ze af
var options = new PrimaveraSaveOptions
                  {
                      // definieer voorvoegsel en achtervoegsel van een activiteit
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // beheers het hernummeren van activiteiten
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Zie ook

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


