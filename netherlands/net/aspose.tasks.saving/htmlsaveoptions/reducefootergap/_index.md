---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "HtmlSaveOptions eigenschap. Haalt een waarde op of stelt deze in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind."
type: docs
weight: 150
url: /nl/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

Haalt op of stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Voorbeelden

Toont hoe een waarde in te stellen die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind in HTML-uitvoerbestanden.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### Zie ook

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


