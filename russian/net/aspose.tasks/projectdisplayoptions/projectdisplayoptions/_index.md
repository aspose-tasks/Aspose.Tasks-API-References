---
title: "ProjectDisplayOptions.ProjectDisplayOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор ProjectDisplayOptions. Инициализирует новый экземпляр класса ProjectDisplayOptions"
type: docs
weight: 10
url: /ru/net/aspose.tasks/projectdisplayoptions/projectdisplayoptions/
---
## ProjectDisplayOptions constructor

Инициализирует новый экземпляр класса [`ProjectDisplayOptions`](../).

```csharp
public ProjectDisplayOptions()
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


