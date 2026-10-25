---
title: "SaveOptions.IsPortrait"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit une valeur indiquant si l'orientation de la page est portrait, renvoie false si l'orientation de la page est paysage."
type: docs
weight: 70
url: /fr/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

Obtient ou définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage.

```csharp
public bool IsPortrait { get; set; }
```

## Remarques

N'est pas applicable lorsque SaveOptions.PageSize == Visualization.PageSize.DefinedInView. Dans ce cas, View.PageInfo.PageSettings.IsPortrait est utilisé à la place. N'est pas applicable lorsque SaveOptions.CustomPageSize est défini.

## Exemples

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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


