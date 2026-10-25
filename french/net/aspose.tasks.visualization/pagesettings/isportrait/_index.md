---
title: "PageSettings.IsPortrait"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageSettings. Obtient ou définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage"
type: docs
weight: 40
url: /fr/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

Obtient ou définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage.

```csharp
public bool IsPortrait { get; set; }
```

## Remarques

Est applicable lors du rendu lorsque SaveOptions.PageSize == Visualization.PageSize.DefinedInView.

## Exemples

Montre comment travailler avec &lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// obtenir les paramètres
var settings = project.DefaultView.PageInfo.PageSettings;
// ajustons quelques propriétés
// définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage.
settings.IsPortrait = true;
// définit le nombre de pages en largeur à imprimer.
settings.PagesInWidth = 5;
// définit le nombre de pages en hauteur à imprimer.
settings.PagesInHeight = 7;
// définit un pourcentage de la taille normale auquel ajuster l'impression.
settings.PercentOfNormalSize = 200;
// définit une taille de papier. Peut être l'une des valeurs de l'énumération <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" />.
settings.PaperSize = PrinterPaperSize.PaperB4;
// définit le numéro de première page pour l'impression.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

Montre comment spécifier la taille et l'orientation de la page en utilisant les paramètres View ou en utilisant SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// Dans ce cas, la taille et l'orientation de la page sont appliquées à partir des propriétés view.PageInfo.PageSettings.PaperSize et view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// Dans ce cas, la taille et l'orientation de la page sont appliquées à partir des propriétés de SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// Dans ce cas, la taille de la page est appliquée à partir de SaveOptions.CustomPageSize. La propriété IsPortrait n'est pas prise en compte.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Voir aussi

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


