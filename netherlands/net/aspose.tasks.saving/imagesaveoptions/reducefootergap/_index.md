---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ImageSaveOptions eigenschap. Haalt een waarde op of stelt deze in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind."
type: docs
weight: 80
url: /nl/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

Haalt op of stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Voorbeelden

Toont hoe je een waarde instelt die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Gebruik de ReduceFooterGap eigenschap om de ruimte tussen de takenlijst en de voettekst te verkleinen.
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### Zie ook

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


