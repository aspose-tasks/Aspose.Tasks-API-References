---
title: "PageLegend.Width"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageLegend. Obtient ou définit la largeur de la partie gauche contenant le nom et la date du projet par défaut de la légende, en centimètres"
type: docs
weight: 30
url: /fr/net/aspose.tasks.visualization/pagelegend/width/
---
## PageLegend.Width property

Obtient ou définit la largeur de la partie gauche (contenant le nom du projet et la date par défaut) de la légende en centimètres.

```csharp
public double Width { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Lorsqu'on tente de définir une valeur inférieure à 0. |

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

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


