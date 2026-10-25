---
title: "ImageSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ImageSaveOptions eigenschap. Haalt een lijst met paginanummers op of stelt deze in die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. Alle pagina's worden opgeslagen als deze lijst leeg is."
type: docs
weight: 50
url: /nl/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

Haalt op of stelt een lijst met paginanummers in die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. Alle pagina's worden opgeslagen als deze lijst leeg is.

```csharp
public List<int> Pages { get; set; }
```

## Voorbeelden

Toont hoe geselecteerde pagina's op te slaan als een afbeelding.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### Zie ook

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


