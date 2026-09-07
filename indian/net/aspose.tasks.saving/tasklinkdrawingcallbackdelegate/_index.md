---
title: "Delegate TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "एक कॉलबैक का प्रतिनिधित्व करता है जो Gantt चार्ट व्यू में कार्य लिंक रेंडर होने पर कॉल किया जाता है।"
type: docs
weight: 2240
url: /hi/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

एक कॉलबैक को दर्शाता है जो गैंट चार्ट दृश्य में टास्क लिंक रेंडर होने पर कॉल किया जाता है।

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | कॉलबैक डेटा को शामिल करने वाली [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) क्लास की इंस्टेंस। |

## उदाहरण

Gantt चार्ट व्यू को रेंडर करते समय कार्य लिंक के रंग को अनुकूलित करने के लिए TaskLinkDrawingCallback का उपयोग कैसे करें, यह दिखाता है।

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

### संबंधित देखें

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


