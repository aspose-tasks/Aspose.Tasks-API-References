---
title: "PageMargins.Borders"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "PageMargins proprietà. Ottiene o imposta una posizione dove stampare i bordi. Può essere uno dei valori dell'enumerazione Border"
type: docs
weight: 20
url: /it/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

Ottiene o imposta una posizione dove stampare i bordi. Può essere uno dei valori dell'enumerazione [`Border`](../../border/).

```csharp
public Border Borders { get; set; }
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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


