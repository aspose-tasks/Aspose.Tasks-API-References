---
title: "مفوض TaskLinkDrawingCallbackDelegate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "يمثل رد اتصال يُستدعى عندما يتم عرض رابط مهمة في منظور مخطط جانت."
type: docs
weight: 2240
url: /ar/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

يمثل رد نداء يتم استدعاؤه عندما يتم عرض رابط المهمة في عرض مخطط جانت.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | مثيل الفئة [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) التي تحتوي على بيانات رد الاتصال. |

## الأمثلة

يوضح كيفية استخدام TaskLinkDrawingCallback لتخصيص لون رابط المهمة عند عرض مخطط جانت.

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

### انظر أيضًا

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


