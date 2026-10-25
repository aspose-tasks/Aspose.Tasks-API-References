---
title: "Delegate TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Bir görev bağlantısı Gantt şeması görünümünde renderlandığında çağrılan bir geri çağırma işlevini temsil eder."
type: docs
weight: 2240
url: /tr/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Gantt şeması görünümünde bir görev bağlantısı oluşturulduğunda çağrılan bir geri aramayı temsil eder.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | Geri çağırma verilerini içeren [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) sınıfının örneği. |

## Örnekler

Gantt şeması görünümünde renderlanırken bir görev bağlantısının rengini özelleştirmek için TaskLinkDrawingCallback'in nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A3;
saveOptions.StartDate = project.StartDate.AddDays(-2);
saveOptions.EndDate = project.FinishDate.AddDays(2);
saveOptions.ViewSettings = view;
saveOptions.TaskLinkDrawingCallback += delegate(TaskLinkDrawingArgs args)
{
    if (args.Link.LinkType == TaskLinkType.FinishToFinish)
    {
        args.Color = Color.Red;
    }
};

project.Save(OutDir + "WorkWithTaskLinkDrawingCallback_out.pdf", saveOptions);
```

### Ayrıca Bakınız

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


