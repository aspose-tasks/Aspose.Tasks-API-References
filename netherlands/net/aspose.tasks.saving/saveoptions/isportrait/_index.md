---
title: "SaveOptions.IsPortrait"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions-eigenschap. Haalt een waarde op of stelt deze in die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is."
type: docs
weight: 70
url: /nl/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

Haalt op of stelt een waarde in die aangeeft of de paginarichting portret is; geeft onwaar terug als de paginarichting landschap is.

```csharp
public bool IsPortrait { get; set; }
```

## Opmerkingen

Is niet van toepassing wanneer SaveOptions.PageSize == Visualization.PageSize.DefinedInView. In dit geval wordt View.PageInfo.PageSettings.IsPortrait gebruikt. Is niet van toepassing wanneer SaveOptions.CustomPageSize is ingesteld.

## Voorbeelden

Toont hoe de paginagrootte en -oriëntatie te specificeren met behulp van View-instellingen of SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// In dit geval worden de paginagrootte en -oriëntatie toegepast vanuit de eigenschappen view.PageInfo.PageSettings.PaperSize en view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// In dit geval worden de paginagrootte en -oriëntatie toegepast vanuit de eigenschappen van SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// In dit geval wordt de paginagrootte toegepast vanuit SaveOptions.CustomPageSize. De IsPortrait-eigenschap wordt niet in aanmerking genomen.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Zie ook

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


