---
title: "SaveOptions.ViewSettings"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Render edilecek bir view (Görünüm) alır veya ayarlar. Bu seçeneği, hangi view'in PDF, HTML veya Image formatlarında kaydedileceğini açıkça belirtmek için kullanabilirsiniz. Bu özellik ayarlandığında proje kaydedilirken PresentationFormat özelliği yoksayılır. View, aşağıdaki ekranlardan biri olmalıdır: Screen, Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage."
type: docs
weight: 240
url: /tr/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Render edilecek bir view ([`View`](../view/)) alır veya ayarlar. Bu seçeneği, hangi view'in PDF, HTML veya Image formatlarında kaydedileceğini açıkça belirtmek için kullanabilirsiniz. Bu özellik ayarlandığında, proje kaydedilirken [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) özelliği yoksayılır. View, aşağıdaki ekranlardan biri olmalıdır (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

```csharp
public View ViewSettings { get; set; }
```

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentException | Ayar yöntemi çağrıldığında ve Screen özelliği desteklenmeyen bir değerle View sınıfının bir örneği sağlandığında. |

## Örnekler

‘SaveOptions.ViewSettings’ kullanılarak render edilmesi gereken view'in nasıl belirtileceğini gösterir.

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

### Ayrıca Bakınız

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


