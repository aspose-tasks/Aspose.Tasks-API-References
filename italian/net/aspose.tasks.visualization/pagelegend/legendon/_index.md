---
title: "PageLegend.LegendOn"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PageLegend. Ottiene o imposta le pagine su cui appare la legenda. Può essere uno dei valori dell'enumerazione Legend"
type: docs
weight: 20
url: /it/net/aspose.tasks.visualization/pagelegend/legendon/
---
## PageLegend.LegendOn property

Ottiene o imposta le pagine su cui appare la legenda. Può essere uno dei valori dell'enumerazione [`Legend`](../../legend/).

```csharp
public Legend LegendOn { get; set; }
```

## Esempi

Mostra come lavorare con le informazioni della legenda della pagina.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// consente di leggere le informazioni della legenda della pagina
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// anche la modifica di una legenda è supportata
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* enum [Legend](../../legend/)
* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


