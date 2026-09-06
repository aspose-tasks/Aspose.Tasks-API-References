---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ImageSaveOptions. Obtient ou définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit"
type: docs
weight: 80
url: /fr/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

Obtient ou définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Exemples

Montre comment définir une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Utilisez la propriété ReduceFooterGap pour réduire l'écart entre la liste des tâches et le pied de page
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### Voir aussi

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


