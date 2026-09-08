---
title: "Project.DefaultWeekWorkingDays"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает экземпляр класса WeekDayCollection, представляющего коллекцию стандартных рабочих дней недели проекта и их рабочее время"
type: docs
weight: 370
url: /ru/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

Получает экземпляр класса [`WeekDayCollection`](../../weekdaycollection/), представляющего коллекцию стандартных рабочих дней недели проекта и их рабочее время.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### Возвращаемое значение

Экземпляр класса [`WeekDayCollection`](../../weekdaycollection/), содержащий список объектов [`WeekDay`](../../weekday/).

## Примечания

Данные содержатся только в файлах mpp (не в xml).

## Примеры

Показывает, как получить стандартный рабочий день недели.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### См. также

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


