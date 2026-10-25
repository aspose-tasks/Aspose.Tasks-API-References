---
title: "Classe PageLegend"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.PageLegend. Représente une légende de page utilisée pour l'impression du projet."
type: docs
weight: 3210
url: /fr/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

Représente une légende de page qui est utilisée pour l'impression du projet.

```csharp
public class PageLegend : HeaderFooterInfo
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageLegend](pagelegend/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Obtient ou définit l'image centrée à afficher dans l'élément parent. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Obtient ou définit la taille affichée de l'image centrale. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Obtient ou définit le texte centré à afficher dans l'élément parent. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Obtient ou définit l'image alignée à gauche à afficher dans l'élément parent. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Obtient ou définit la taille affichée de l'image de gauche. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Obtient ou définit le texte aligné à gauche à afficher dans l'élément parent. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | Obtient ou définit les pages sur lesquelles la légende apparaît. Peut être l'une des valeurs de l'énumération [`Legend`](../legend/). |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Obtient ou définit l'image alignée à droite à afficher dans l'élément parent. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Obtient ou définit la taille affichée de l'image de droite. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Obtient ou définit le texte aligné à droite à afficher dans l'élément parent. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | Obtient ou définit la largeur de la partie gauche (contenant le nom du projet et la date par défaut) de la légende en centimètres. |

## Exemples

Montre comment travailler avec les informations de légende de page.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// lisons les informations de légende de page
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// la modification d'une légende est également prise en charge
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


