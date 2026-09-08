---
title: "SaveOptions.TaskLinkDrawingCallback"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает обратный вызов, который можно использовать для настройки некоторых аспектов рендеринга связей задач."
type: docs
weight: 180
url: /ru/net/aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/
---
## SaveOptions.TaskLinkDrawingCallback property

Получает или задает обратный вызов, который можно использовать для настройки некоторых аспектов отрисовки связей задач.

```csharp
public TaskLinkDrawingCallbackDelegate TaskLinkDrawingCallback { get; set; }
```

## Примечания

Применяется только при рендеринге представления диаграммы Ганта.

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

* delegate [TaskLinkDrawingCallbackDelegate](../../tasklinkdrawingcallbackdelegate/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


