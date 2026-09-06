---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PdfSaveOptions. Obtient ou définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit"
type: docs
weight: 80
url: /fr/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

Obtient ou définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Exemples

Montre comment définir une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit dans les fichiers PDF de sortie.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### Voir aussi

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


