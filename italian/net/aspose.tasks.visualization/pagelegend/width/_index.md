---
title: "PageLegend.Width"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PageLegend. Ottiene o imposta la larghezza della parte sinistra contenente il nome e la data del progetto per impostazione predefinita della legenda, in centimetri"
type: docs
weight: 30
url: /it/net/aspose.tasks.visualization/pagelegend/width/
---
## PageLegend.Width property

Ottiene o imposta la larghezza della parte sinistra (che contiene per impostazione predefinita il nome e la data del progetto) della legenda in centimetri.

```csharp
public double Width { get; set; }
```

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | Quando si tenta di impostare un valore inferiore a 0. |

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

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


