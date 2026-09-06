---
title: "SaveOptions.ViewSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit une vue View à rendre. Vous pouvez utiliser cette option pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image. Si cette propriété est définie, la propriété PresentationFormat est ignorée lors de l'enregistrement du projet. La vue doit provenir de l'un des écrans suivants : Screen Gantt TaskSheet TaskUsage ResourceSheet ResourceUsage."
type: docs
weight: 240
url: /fr/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Obtient ou définit une vue ([`View`](../view/)) à rendre. Vous pouvez utiliser cette option pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image. Si cette propriété est définie, la propriété [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) est ignorée lors de l'enregistrement du projet. La vue doit provenir de l'un des écrans suivants (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

```csharp
public View ViewSettings { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lorsque la méthode set est appelée et qu'une instance de la classe View avec une valeur non prise en charge de la propriété Screen est fournie. |

## Exemples

Montre comment utiliser 'SaveOptions.ViewSettings' pour spécifier la vue qui doit être rendue en PDF.

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

### Voir aussi

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


