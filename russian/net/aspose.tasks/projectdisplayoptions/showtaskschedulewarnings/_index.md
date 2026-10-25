---
title: "ProjectDisplayOptions.ShowTaskScheduleWarnings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ProjectDisplayOptions. Получает или задает значение, указывающее, следует ли показывать предупреждения, когда Project обнаруживает возможный конфликт планирования с вручную запланированной задачей. Эта опция доступна, начиная с версии Project 2010 и позже"
type: docs
weight: 90
url: /ru/net/aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/
---
## ProjectDisplayOptions.ShowTaskScheduleWarnings property

Получает или задает значение, указывающее, следует ли показывать предупреждения, когда Project обнаруживает возможный конфликт планирования с вручную запланированной задачей. Эта опция доступна в версии Project 2010 и позже.

```csharp
public bool ShowTaskScheduleWarnings { get; set; }
```

## Примеры

Показывает, как использовать параметры отображения проекта.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Задайте значение, указывающее, следует ли показывать предупреждения, когда Project обнаруживает возможный конфликт планирования с вручную запланированной задачей.
// Эта опция доступна в версии Project 2010 и позже.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// значение, указывающее, следует ли добавлять пробел перед числовым значением и сокращением времени (1 wk вместо 1wk)
project.DisplayOptions.AddSpaceBeforeLabel = true;

// устанавливает, как отображается метка минут
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// установить, как отображается метка часа
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// задать способ отображения метки дня
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// задать способ отображения метки недели
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// установить, как отображается метка месяца
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// установить, как отображается метка года
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// задать значение, указывающее, следует ли отображать сводную информацию о полном проекте в одной строке со своей полосой сводной задачи в верхней части представления диаграммы Ганта.
project.DisplayOptions.ShowProjectSummaryTask = true;

// задать значение, указывающее, следует ли показывать предложения, когда Project обнаруживает возможный конфликт планирования с вручную запланированной задачей.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// задать значение, указывающее, следует ли подчеркивать гиперссылки.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [ProjectDisplayOptions](../)
* namespace [Aspose.Tasks](../../projectdisplayoptions/)
* assembly [Aspose.Tasks](../../../)


