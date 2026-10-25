---
title: "Делегат TaskLinkDrawingCallbackDelegate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Представляет обратный вызов, который вызывается при отрисовке связи задачи в представлении диаграммы Ганта."
type: docs
weight: 2240
url: /ru/net/aspose.tasks.saving/tasklinkdrawingcallbackdelegate/
---
## TaskLinkDrawingCallbackDelegate delegate

Представляет обратный вызов, который вызывается при рендеринге ссылки задачи в представлении диаграммы Ганта.

```csharp
public delegate void TaskLinkDrawingCallbackDelegate(TaskLinkDrawingArgs args);
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| args | TaskLinkDrawingArgs | экземпляр класса [`TaskLinkDrawingArgs`](../../aspose.tasks/tasklinkdrawingargs/), содержащий данные обратного вызова. |

## Примеры

Показывает, как использовать TaskLinkDrawingCallback для настройки цвета связи задачи при отрисовке представления диаграммы Ганта.

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

### См. также

* class [TaskLinkDrawingArgs](../../aspose.tasks/tasklinkdrawingargs/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


