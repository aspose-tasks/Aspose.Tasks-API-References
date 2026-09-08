---
title: "Enum Border"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.Border enum. Specificeert het type randen."
type: docs
weight: 2970
url: /nl/net/aspose.tasks.visualization/border/
---
## Border enumeration

Specificeert het type randen.

```csharp
public enum Border
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| NoBorder | `0` | Geen rand. |
| AroundEveryPage | `1` | Rond elke pagina. |
| OutsidePages | `2` | Op de buitenste pagina's. |

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


