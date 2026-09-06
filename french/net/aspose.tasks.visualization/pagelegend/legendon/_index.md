---
title: "PageLegend.LegendOn"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PageLegend. Obtient ou définit les pages sur lesquelles la légende apparaît. Peut être l'une des valeurs de l'énumération Legend"
type: docs
weight: 20
url: /fr/net/aspose.tasks.visualization/pagelegend/legendon/
---
## PageLegend.LegendOn property

Obtient ou définit les pages sur lesquelles la légende apparaît. Peut être l'une des valeurs de l'énumération [`Legend`](../../legend/).

```csharp
public Legend LegendOn { get; set; }
```

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

* enum [Legend](../../legend/)
* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


