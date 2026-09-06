---
title: "PageSettings.PagesInHeight"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageSettings. Obtient ou définit un nombre de pages en hauteur à imprimer"
type: docs
weight: 50
url: /fr/net/aspose.tasks.visualization/pagesettings/pagesinheight/
---
## PageSettings.PagesInHeight property

Obtient ou définit le nombre de pages en hauteur à imprimer.

```csharp
public int PagesInHeight { get; set; }
```

## Exemples

Montre comment rendre la vue avec l'option 'Fit X to Y pages'.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// spécifier que la vue doit être rendue en 2 pages ou moins en hauteur
view.PageInfo.PageSettings.PagesInHeight = 2;
// spécifier que la vue doit être rendue en 1 page en largeur
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### Voir aussi

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


