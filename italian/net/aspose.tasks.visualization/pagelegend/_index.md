---
title: "Classe PageLegend"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.PageLegend. Rappresenta una legenda della pagina utilizzata per la stampa del progetto."
type: docs
weight: 3210
url: /it/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

Rappresenta una legenda di pagina utilizzata per la stampa del progetto.

```csharp
public class PageLegend : HeaderFooterInfo
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PageLegend](pagelegend/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Ottiene o imposta l'immagine centrata da visualizzare nell'elemento genitore. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Ottiene o imposta la dimensione visualizzata dell'immagine centrale. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Ottiene o imposta il testo centrato da visualizzare nell'elemento genitore. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Ottiene o imposta l'immagine allineata a sinistra da visualizzare nell'elemento padre. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Ottiene o imposta la dimensione visualizzata dell'immagine a sinistra. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Ottiene o imposta il testo allineato a sinistra da visualizzare nell'elemento padre. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | Ottiene o imposta le pagine su cui appare la legenda. Può essere uno dei valori dell'enumerazione [`Legend`](../legend/). |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Ottiene o imposta l'immagine allineata a destra da visualizzare nell'elemento padre. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Ottiene o imposta la dimensione visualizzata dell'immagine a destra. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Ottiene o imposta il testo allineato a destra da visualizzare nell'elemento padre. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | Ottiene o imposta la larghezza della parte sinistra (che contiene per impostazione predefinita il nome e la data del progetto) della legenda in centimetri. |

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

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


