---
title: "Класс CalendarException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.CalendarException. Представляет исключительные периоды времени в календаре"
type: docs
weight: 250
url: /ru/net/aspose.tasks/calendarexception/
---
## CalendarException class

Представляет исключительные периоды времени в календаре.

```csharp
public sealed class CalendarException
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CalendarException](calendarexception/)() | Инициализирует новый экземпляр класса `CalendarException`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Возвращает DayTypeCollection для этого объекта. Дни недели, в которые исключение действительно. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Получает или задает значение, указывающее, является ли указанная дата или тип дня рабочим. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Получает или задает значение, указывающее, определяется ли диапазон повторения вводом количества повторений. Значение False указывает, что диапазон повторения определяется вводом даты завершения. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Получает или задает начало времени исключения. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Получает или задает месяц, для которого запланировано повторение исключения. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Получает или задает день месяца, в который запланировано повторение исключения. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Получает или задает элемент месяца, для которого запланировано повторение исключения. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Получает или задает позицию элемента месяца внутри месяца. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Получает или задает имя исключения. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Получает или задает количество повторений, в течение которых исключение календаря действительно. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Получает родительский календарь для этого объекта. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Получает или задает период повторения для исключения. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Получает или задает конец времени исключения. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Получает или задает тип исключения. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Получает или задает объект WorkingTimeCollection. Коллекция рабочих времён, определяющая время работы в будний день. Должно присутствовать как минимум одно рабочее время, и их не может быть более пяти. |

## Методы

| Имя | Описание |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Возвращает true, если указанная экземпляр структуры DateTime является днём исключения. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Удаляет экземпляр Exception из родительского объекта календаря CalendarExceptionCollection. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Возвращает даты, на которые применяется исключение календаря. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Возвращает рабочее время для исключения календаря. |

## Примеры

Показывает, как добавлять/удалять исключения календаря.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// создать календарь
var calendar = project.Calendars.Add("Calendar1");

// создать исключение будних дней для праздника
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// проверить, что дата является исключительной
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// удалить исключение
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// добавить исключение
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// вывести исключения
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


