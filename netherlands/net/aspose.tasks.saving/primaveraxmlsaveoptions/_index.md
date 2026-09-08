---
title: "Klasse PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.PrimaveraXmlSaveOptions‑klasse. Hiermee kunt u extra opties opgeven bij het opslaan van een project naar het Primavera‑xml‑formaat"
type: docs
weight: 2160
url: /nl/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

Staat toe extra opties op te geven bij het opslaan van een project naar het Primavera XML‑formaat.

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | Initialiseert een nieuw exemplaar van de `PrimaveraXmlSaveOptions`‑klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Haalt op of stelt het formaat in waarin het document wordt opgeslagen als dit opslaanopties‑object wordt gebruikt. |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of een hoofdtaak moet worden opgeslagen of niet. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Haalt op of stelt de comparer in om taken te sorteren op het Gantt‑diagram en het Task‑Sheet‑diagram. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Haalt op of stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden gerenderd op Gantt‑, Task‑Sheet‑ en Task‑Usage‑diagrammen. |

## Voorbeelden

Toont hoe te exporteren naar een Primavera‑XML‑bestand.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Zie ook

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


