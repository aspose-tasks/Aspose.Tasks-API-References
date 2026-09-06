---
title: "ImageSaveOptions.Pages"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ImageSaveOptions. Obtient ou définit une liste de numéros de pages à enregistrer lors de l'enregistrement de la mise en page du projet dans des fichiers séparés. Toutes les pages seront enregistrées si cette liste est vide"
type: docs
weight: 50
url: /fr/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

Obtient ou définit une liste de numéros de pages à enregistrer lors de la sauvegarde de la mise en page du projet dans des fichiers séparés. Toutes les pages seront enregistrées si cette liste est vide.

```csharp
public List<int> Pages { get; set; }
```

## Exemples

Montre comment enregistrer les pages sélectionnées en tant qu'image.

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

### Voir aussi

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


