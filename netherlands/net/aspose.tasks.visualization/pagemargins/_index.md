---
title: "Klasse PageMargins"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.PageMargins klasse. Vertegenwoordigt paginamarges voor afdrukken"
type: docs
weight: 3230
url: /nl/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

Stelt paginamarges voor afdrukken voor.

```csharp
public class PageMargins
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PageMargins](pagemargins/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | Haalt op of stelt een positie in waar randen worden afgedrukt. Kan een van de waarden van de [`Border`](../border/) enumeratie zijn. |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | Haalt op of stelt de grootte van de onderste marge in centimeters in. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | Haalt op of stelt de grootte van de linkermarge in centimeters in. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | Haalt op of stelt de grootte van de rechtermarge in centimeters in. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | Haalt op of stelt de grootte van de bovenste marge in centimeters in. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


