---
title: "PageSettings.PageSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur PageSettings. Initialise une nouvelle instance de la classe PageSettings. Représente les paramètres d'impression pour une page de la vue du projet."
type: docs
weight: 10
url: /fr/net/aspose.tasks.visualization/pagesettings/pagesettings/
---
## PageSettings constructor

Initialise une nouvelle instance de la classe [`PageSettings`](../). Représente les paramètres d'impression pour une page de la vue du projet.

```csharp
public PageSettings()
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

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


