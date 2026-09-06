---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageSettings. Obtient ou définit une valeur indiquant s'il faut ajuster l'impression au pourcentage spécifié PercentOfNormalSize de la taille normale"
type: docs
weight: 20
url: /fr/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

Obtient ou définit une valeur indiquant s'il faut ajuster l'impression au pourcentage spécifié ([`PercentOfNormalSize`](../percentofnormalsize/)) de la taille normale.

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## Remarques

N'est pas efficace lorsque le projet est rendu au format HTML.

## Exemples

Montre comment rendre la vue avec le facteur d'échelle spécifié.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// définir une valeur indiquant que la vue doit être mise à l'échelle en utilisant le facteur d'échelle spécifié
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// spécifier le facteur d'échelle
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### Voir aussi

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


