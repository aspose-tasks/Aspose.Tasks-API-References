---
title: "SaveOptions.ViewSettings"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions-eigenschap. Haalt een view (View) op of stelt deze in om te renderen. U kunt deze optie gebruiken om expliciet op te geven welke view moet worden opgeslagen in PDF-, HTML- of afbeeldingsformaten. Als deze eigenschap is ingesteld, wordt de PresentationFormat-eigenschap genegeerd wanneer het project wordt opgeslagen. De view moet afkomstig zijn van een van de volgende schermen: Screen Gantt TaskSheet TaskUsage ResourceSheet ResourceUsage."
type: docs
weight: 240
url: /nl/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Haalt een view ([`View`](../view/)) op of stelt deze in om te renderen. U kunt deze optie gebruiken om expliciet op te geven welke view moet worden opgeslagen in PDF-, HTML- of afbeeldingsformaten. Als deze eigenschap is ingesteld, wordt de [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) eigenschap genegeerd wanneer het project wordt opgeslagen. De view moet afkomstig zijn van een van de volgende schermen (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

```csharp
public View ViewSettings { get; set; }
```

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentException | Wanneer de set-methode wordt aangeroepen en een instantie van de View-klasse met een niet-ondersteunde waarde van de Screen-eigenschap wordt opgegeven. |

## Voorbeelden

Toont hoe 'SaveOptions.ViewSettings' te gebruiken om de view te specificeren die naar PDF moet worden gerenderd.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);
Console.WriteLine("Page size specified in view settings: " + view.PageInfo.PageSettings.PaperSize);
Console.WriteLine("Page orientation: {0}", view.PageInfo.PageSettings.IsPortrait ? "Portrait" : "Landscape");

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.DefinedInView;
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

project.Save(OutDir + "SaveToPdfUsingSpecificView_out.pdf", saveOptions);
```

### Zie ook

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


