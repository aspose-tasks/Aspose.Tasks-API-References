---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PdfSaveOptions-eigenschap. Haalt op of stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind."
type: docs
weight: 80
url: /nl/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

Haalt op of stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Voorbeelden

Toont hoe een waarde in te stellen die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind in PDF-uitvoerbestanden.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### Zie ook

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


