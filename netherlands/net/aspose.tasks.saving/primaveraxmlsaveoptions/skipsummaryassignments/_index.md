---
title: "PrimaveraXmlSaveOptions.SkipSummaryAssignments"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraXmlSaveOptions eigenschap. Haalt een waarde op of stelt deze in die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export"
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/
---
## PrimaveraXmlSaveOptions.SkipSummaryAssignments property

Haalt een waarde op of stelt deze in die aangeeft of toewijzingen van resources aan samenvattende taken moeten worden overgeslagen tijdens export.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Opmerkingen

Primavera‑software ondersteunt geen toewijzingen van resources aan samenvattende (WBS) taken. Daarom kan het exporteren van dergelijke toewijzingen leiden tot een ongeldig bestand volgens het model van Primavera. Als true, worden toewijzingen aan samenvattende taken overgeslagen tijdens export. Als false (de standaardwaarde), wordt er een uitzondering gegooid als tijdens export een toewijzing aan een samenvattende taak wordt aangetroffen.

## Voorbeelden

Toont hoe de SkipSummaryAssignments‑vlag te gebruiken.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera ondersteunt geen toewijzingen van resources aan samenvattende taken.
// Het exporteren van dergelijke toewijzingen naar het Primavera-formaat kan resulteren in bestanden die niet in Primavera geïmporteerd kunnen worden.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### Zie ook

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


