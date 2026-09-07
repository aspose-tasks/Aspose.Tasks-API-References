---
title: "PageMargins.Left"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "PageMargins proprietà. Ottiene o imposta la dimensione del margine sinistro in centimetri"
type: docs
weight: 40
url: /it/net/aspose.tasks.visualization/pagemargins/left/
---
## PageMargins.Left property

Ottiene o imposta la dimensione del margine sinistro in centimetri.

```csharp
public double Left { get; set; }
```

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

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


