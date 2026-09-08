---
title: "Класс ProjectDisplayOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ProjectDisplayOptions. Представляет параметры отображения для экземпляра проекта."
type: docs
weight: 1450
url: /ru/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

Представляет параметры отображения экземпляра проекта.

```csharp
public class ProjectDisplayOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | Инициализирует новый экземпляр класса `ProjectDisplayOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | Получает или задает значение, указывающее, следует ли добавлять пробел перед числовым значением и сокращением времени (1 wk вместо 1wk). |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | Получает или задает отображение метки дня. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | Получает или задает отображение метки часа. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | Получает или задает отображение метки минуты. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | Получает или задает отображение метки месяца. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | Получает или задает значение, указывающее, следует ли отображать сводную информацию о полном проекте в одной строке со своей полосой сводной задачи в верхней части представления диаграммы Ганта. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | Получает или задает значение, указывающее, следует ли показывать предложения, когда Project обнаруживает возможный конфликт планирования с вручную запланированной задачей. Эта опция доступна в версии Project 2010 и позже. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | Получает или задает значение, указывающее, следует ли показывать предупреждения, когда Project обнаруживает возможный конфликт планирования с вручную запланированной задачей. Эта опция доступна в версии Project 2010 и позже. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | Получает или задает значение, указывающее, следует ли подчеркивать гиперссылки. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | Получает или задает способ отображения метки недели. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | Получает или задает способ отображения метки года. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


