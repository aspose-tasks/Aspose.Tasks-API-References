---
title: "PageMargins.Left"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageMargins property. Geeft of stelt de grootte van de linker marge in centimeters."
type: docs
weight: 40
url: /nl/net/aspose.tasks.visualization/pagemargins/left/
---
## PageMargins.Left property

Haalt op of stelt de grootte van de linkermarge in centimeters in.

```csharp
public double Left { get; set; }
```

## Voorbeelden

Toont hoe te werken met paginamarges.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// laat de standaardweergave aanpassen
var margins = project.DefaultView.PageInfo.Margins;

// laat marges aanpassen
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


