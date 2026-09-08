---
title: "PageMargins.Borders"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PageMargins-eigenschap. Haalt op of stelt een positie in waar grenzen moeten worden afgedrukt. Kan een van de waarden van de Border-enumeratie zijn."
type: docs
weight: 20
url: /nl/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

Geeft of stelt een positie in waarop randen worden afgedrukt. Kan een van de waarden van de [`Border`](../../border/) enumeratie zijn.

```csharp
public Border Borders { get; set; }
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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


