---
title: "PageSettings.PercentOfNormalSize"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageSettings. Obtient ou définit un pourcentage de la taille normale pour ajuster l'impression à"
type: docs
weight: 90
url: /fr/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

Obtient ou définit un pourcentage de la taille normale auquel ajuster l'impression.

```csharp
public int PercentOfNormalSize { get; set; }
```

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


