---
title: "SaveOptions.TaskLinkDrawingCallback"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Görev bağlantılarının render edilmesinin bazı yönlerini özelleştirmek için kullanılabilecek bir geri çağırma işlevini alır veya ayarlar."
type: docs
weight: 180
url: /tr/net/aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/
---
## SaveOptions.TaskLinkDrawingCallback property

Görev bağlantılarının renderlanmasının bazı yönlerini özelleştirmek için kullanılabilecek bir geri çağırma işlevini alır veya ayarlar.

```csharp
public TaskLinkDrawingCallbackDelegate TaskLinkDrawingCallback { get; set; }
```

## Açıklamalar

Yalnızca Gantt şeması görünümü render edildiğinde uygulanır.

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

* delegate [TaskLinkDrawingCallbackDelegate](../../tasklinkdrawingcallbackdelegate/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


