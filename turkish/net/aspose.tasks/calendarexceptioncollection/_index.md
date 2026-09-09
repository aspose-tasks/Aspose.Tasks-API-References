---
title: "Sınıf CalendarExceptionCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CalendarExceptionCollection sınıfı. CalendarException nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 260
url: /tr/net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

[`CalendarException`](../calendarexception/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | `CalendarExceptionCollection` nesnesinde bulunan nesne sayısını alır. |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür. |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | Bu nesne için üst takvimi alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | Bu koleksiyon nesnesine CalendarException örneği ekler. |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | İç listeye istisna aralığını ekler. |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | `CalendarExceptionCollection` içindeki tüm öğeleri kaldırır. |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | Bu koleksiyondan [`CalendarException`](../calendarexception/) örneğini kaldırır. |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | CalendarExceptionCollection nesnesini [`CalendarException`](../calendarexception/) nesnelerinin bir listesine dönüştürür. |

## Örnekler

Takvim istisna koleksiyonunu kullanarak takvim istisnalarını tanımlamayı gösterir.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByUid(3);

calendar.Exceptions.Clear();
Calendar.MakeStandardCalendar(calendar);

var exception = new CalendarException();
exception.FromDate = new DateTime(2020, 3, 30, 8, 0, 0);
exception.ToDate = new DateTime(2020, 4, 3, 17, 0, 0);
exception.DayWorking = true;
exception.Name = "Exception 1";

var wt1 = new WorkingTime(9, 13);
var wt2 = new WorkingTime(14, 19);

exception.WorkingTimes.Add(wt1);
exception.WorkingTimes.Add(wt2);
calendar.Exceptions.Add(exception);

var nonWorkingExceptions = new CalendarException[2];
nonWorkingExceptions[0] = new CalendarException();
nonWorkingExceptions[0].FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
nonWorkingExceptions[0].ToDate = new DateTime(2020, 4, 18, 17, 0, 0);
nonWorkingExceptions[0].DayWorking = false;
nonWorkingExceptions[0].Name = "Exception 2";
nonWorkingExceptions[1] = new CalendarException();
nonWorkingExceptions[1].FromDate = new DateTime(2020, 4, 6, 8, 0, 0);
nonWorkingExceptions[1].ToDate = new DateTime(2020, 4, 10, 17, 0, 0);
nonWorkingExceptions[1].DayWorking = false;
nonWorkingExceptions[1].Name = "Exception 3";
calendar.Exceptions.AddRange(nonWorkingExceptions);

Console.WriteLine("Exceptions of calendar {0}: ", calendar.Exceptions.ParentCalendar.Name);
Console.WriteLine("Exceptions count: {0}", calendar.Exceptions.Count);
Console.WriteLine();
foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Name: " + calendarException.Name);
    Console.WriteLine("From Date: " + calendarException.FromDate);
    Console.WriteLine("To Date: " + calendarException.ToDate);
    Console.WriteLine("Is day working: " + calendarException.DayWorking);
    Console.WriteLine();
}

// tüm istisnaları kaldır
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### Ayrıca Bakınız

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


