---
title: "UsageView.TopTimescaleTier"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство UsageView. Получает или задает настройки верхнего уровня шкалы времени представления. TimescaleTier"
type: docs
weight: 80
url: /ru/net/aspose.tasks/usageview/toptimescaletier/
---
## UsageView.TopTimescaleTier property

Получает или задает настройки верхнего уровня шкалы времени представления. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
```

## Примеры

Показывает, как отобразить представление использования задач с настройками шкалы времени, определенными в настройках представления.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Определите SaveOptions и укажите, что следует использовать настройки масштаба времени TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### См. также

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


