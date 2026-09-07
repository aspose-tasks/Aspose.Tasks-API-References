---
title: "ImageSaveOptions.Pages"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ImageSaveOptions. Ottiene o imposta un elenco di numeri di pagina da salvare quando si salva il layout del progetto in file separati. Tutte le pagine verranno salvate se questo elenco è vuoto"
type: docs
weight: 50
url: /it/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

Ottiene o imposta un elenco di numeri di pagina da salvare quando il layout del progetto viene salvato in file separati. Tutte le pagine verranno salvate se questo elenco è vuoto.

```csharp
public List<int> Pages { get; set; }
```

## Esempi

Mostra come salvare le pagine selezionate come immagine.

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

### Vedi anche

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


