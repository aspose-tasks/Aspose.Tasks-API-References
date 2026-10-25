---
title: "デリゲート TaskLinkDrawingCallbackDelegate"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "ガントチャートビューでタスクリンクが描画される際に呼び出されるコールバックを表します"
type: docs
weight: 2240
url: /ja/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

ガントチャートビューでタスクリンクが描画される際に呼び出されるコールバックを表します。

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | コールバックデータを含む [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/) クラスのインスタンスです。 |

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

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


