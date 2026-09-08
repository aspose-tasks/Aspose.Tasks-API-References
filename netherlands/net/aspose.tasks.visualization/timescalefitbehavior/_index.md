---
title: "Enum TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.TimescaleFitBehavior-enum. Stelt een gedrag voor dat wordt gebruikt om het tijdschalengebied uit te lijnen met de paginabreedte."
type: docs
weight: 3440
url: /nl/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

Stelt een gedrag voor dat wordt gebruikt om het tijdschaalgebied uit te lijnen met de paginabreedte.

```csharp
public enum TimescaleFitBehavior
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| DefinedInView | `0` | Kalendersectie wordt gerenderd volgens de eigenschap View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage van de gerenderde weergave. |
| NoScaleToEndDate | `1` | Kalendersectie wordt precies tot EndDate gerenderd, zelfs wanneer er een lege ruimte op een pagina is. |
| NoScaleToEndOfPage | `2` | Kalendersectie wordt gerenderd tot het einde (rechterkant) van de laatste pagina. Hierdoor kan de laatst gerenderde datum EndDate overschrijden. |
| ScaleToEndOfPage | `3` | Renderengine zal proberen datums uit te lijnen zodat EndDate is uitgelijnd met het einde (rechterkant) van de laatste pagina. Komt overeen met de ingeschakelde optie "Pagina-instelling \ View \ Fit timescale to end of page" van MS Project. |

## Voorbeelden

Toont hoe TimescaleFitBehavior te gebruiken om de tijdschaal van het Gantt-diagram aan te passen aan het einde van de laatste pagina.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


