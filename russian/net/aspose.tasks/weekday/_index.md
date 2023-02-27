---
title: Class WeekDay
second_title: Справочник по Aspose.Tasks для .NET API
description: Aspose.Tasks.WeekDay сорт. Представляет день недели который определяет обычные дни недели или дни исключения в календаре.
type: docs
weight: 3180
url: /ru/net/aspose.tasks/weekday/
---
## WeekDay class

Представляет день недели, который определяет обычные дни недели или дни исключения в календаре.

```csharp
public class WeekDay
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Инициализирует новый экземпляр`WeekDay` класс. |
| [WeekDay](weekday/#constructor_1)(DayType) | Инициализирует новый экземпляр`WeekDay` класс с указанным типом дня. |
| [WeekDay](weekday/#constructor_2)(DayType, IEnumerable&lt;WorkingTime&gt;) | Инициализирует новый экземпляр`WeekDay` класс с указанным типом дня и списком периодов рабочего времени. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Получает тип дня. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Получает или задает значение, указывающее, работает ли указанная дата или тип дня. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Получает или задает начало времени исключения. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Получает или задает время окончания исключения. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Получает коллекцию WorkingTimeCollection для этого экземпляра WeekDay. Коллекция рабочего времени, определяющая время, отработанное в будний день. |

## Методы

| Имя | Описание |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Создает рабочий день по умолчанию. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Возвращает полную копию дня недели. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Возвращает значение хеш-кода для экземпляра`WeekDay` класс. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Возвращает рабочее время для дня недели. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Преобразует .NetDayOfWeek к[`DayType`](./daytype/) . |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Устанавливает периоды времени по умолчанию для указанного дня недели. |

### Смотрите также

* пространство имен [Aspose.Tasks](../../aspose.tasks/)
* сборка [Aspose.Tasks](../../)


