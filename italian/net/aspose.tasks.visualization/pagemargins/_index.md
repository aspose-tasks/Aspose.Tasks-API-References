---
title: "Classe PageMargins"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.PageMargins. Rappresenta i margini di pagina per la stampa"
type: docs
weight: 3230
url: /it/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

Rappresenta i margini della pagina per la stampa.

```csharp
public class PageMargins
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PageMargins](pagemargins/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | Ottiene o imposta una posizione dove stampare i bordi. Può essere uno dei valori dell'enumerazione [`Border`](../border/). |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | Ottiene o imposta la dimensione del margine inferiore in centimetri. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | Ottiene o imposta la dimensione del margine sinistro in centimetri. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | Ottiene o imposta la dimensione del margine destro in centimetri. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | Ottiene o imposta la dimensione del margine superiore in centimetri. |

## Esempi

Mostra come lavorare con i margini di pagina.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// consente di modificare la vista predefinita
var margins = project.DefaultView.PageInfo.Margins;

// consente di modificare i margini
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


