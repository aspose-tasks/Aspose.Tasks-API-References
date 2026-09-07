---
title: "SaveOptions.ViewSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta una vista View da renderizzare. È possibile utilizzare questa opzione per specificare esplicitamente quale vista deve essere salvata nei formati PDF, HTML o Image. Se questa proprietà è impostata, la proprietà PresentationFormat viene ignorata quando il progetto viene salvato. La vista deve provenire da una delle seguenti schermate Screen: Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage."
type: docs
weight: 240
url: /it/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Ottiene o imposta una vista ([`View`](../view/)) da renderizzare. È possibile utilizzare questa opzione per specificare esplicitamente quale vista deve essere salvata nei formati PDF, HTML o Image. Se questa proprietà è impostata, la proprietà [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) viene ignorata quando il progetto viene salvato. La vista deve provenire da una delle seguenti schermate (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

```csharp
public View ViewSettings { get; set; }
```

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Quando il metodo set viene chiamato e viene fornita un'istanza della classe View con un valore non supportato della proprietà Screen. |

## Esempi

Mostra come utilizzare 'SaveOptions.ViewSettings' per specificare la vista che deve essere renderizzata in PDF.

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

### Vedi anche

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


