---
title: "RecurringInterval.DailyWorkday"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство RecurringInterval. Возвращает или задает значение, указывающее, является ли день рабочим для ежедневных линий прогресса"
type: docs
weight: 30
url: /ru/net/aspose.tasks.visualization/recurringinterval/dailyworkday/
---
## RecurringInterval.DailyWorkday property

Получает или задает значение, указывающее, является ли день рабочим для ежедневных линий прогресса.

```csharp
public bool DailyWorkday { get; set; }
```

## Примеры

Показывает, как добавить ежедневный повторяющийся интервал линий прогресса.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// установить номер дня ежедневного шаблона
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// установить значение, указывающее, является ли день рабочим для ежедневных линий прогресса.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### См. также

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


