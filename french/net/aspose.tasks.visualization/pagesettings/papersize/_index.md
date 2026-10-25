---
title: "PageSettings.PaperSize"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageSettings. Obtient ou définit une taille de papier. Peut être l'une des valeurs de l'énumération PrinterPaperSize"
type: docs
weight: 70
url: /fr/net/aspose.tasks.visualization/pagesettings/papersize/
---
## PageSettings.PaperSize property

Obtient ou définit une taille de papier. Peut être l'une des valeurs de l'énumération [`PrinterPaperSize`](../../printerpapersize/).

```csharp
public PrinterPaperSize PaperSize { get; set; }
```

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

### Voir aussi

* enum [PrinterPaperSize](../../printerpapersize/)
* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


