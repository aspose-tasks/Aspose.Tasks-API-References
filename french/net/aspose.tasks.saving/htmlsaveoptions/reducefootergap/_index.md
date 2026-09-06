---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété HtmlSaveOptions. Obtient ou définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit."
type: docs
weight: 150
url: /fr/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

Obtient ou définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Exemples

Montre comment définir une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit dans les fichiers de sortie HTML.

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

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


