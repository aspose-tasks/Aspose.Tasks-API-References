---
title: "SaveOptions.TaskLinkDrawingCallback"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "SaveOptions プロパティ。タスクリンクの描画のいくつかの側面をカスタマイズできるコールバックを取得または設定します"
type: docs
weight: 180
url: /ja/net/aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/
---
## SaveOptions.TaskLinkDrawingCallback property

タスクリンクの描画のいくつかの側面をカスタマイズできるコールバックを取得または設定します。

```csharp
public TaskLinkDrawingCallbackDelegate TaskLinkDrawingCallback { get; set; }
```

## 備考

Gantt チャートビューがレンダリングされる場合にのみ適用されます。

## 例

ガントチャートビューを描画する際にタスクリンクの色をカスタマイズするために TaskLinkDrawingCallback を使用する方法を示します。

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

### 関連項目

* delegate [TaskLinkDrawingCallbackDelegate](../../tasklinkdrawingcallbackdelegate/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


