---
title: "ICalendar arabirimi"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ICalendar arabirimi. Tarih ve sürelerin çeşitli hesaplamalarında kullanılabilecek bir takvim soyutlamasını temsil eder."
type: docs
weight: 840
url: /tr/net/aspose.tasks/icalendar/
---
## ICalendar interface

Tarih ve sürelerin çeşitli hesaplamaları için kullanılabilecek bir takvim soyutlamasını temsil eder.

```csharp
public interface ICalendar
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Takvime göre belirtilen çalışma süresi miktarı geçtiğinde tarihi hesaplar. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | Belirtilen tarih için bir sonraki çalışma gününün başlangıcını hesaplar. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | Belirtilen tarihten önceki çalışma gününün sonunu hesaplar. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Belirtilen bitiş tarihi ve süreye dayanarak başlangıç tarihini döndürür. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Belirtilen bitiş tarihi ve süreye dayanarak başlangıç tarihini döndürür. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Görevin başlangıç tarihi, bölünmüş parçaları ve çalışma süresinden görev bitiş tarih ve saatini hesaplar. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | Belirtilen tarihteki çalışma saatlerinin miktarını döndürür. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | WorkUnit - Belirtilen tarih zaman aralığı için çalışma saatlerinin Başlangıç, Bitiş ve Süresini döndürür. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | Belirtilen tarihler arasındaki çalışma saatlerinin miktarını döndürür. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Belirtilen tarih için çalışma zamanlarının [`WorkingTimeCollection`](../workingtimecollection/) koleksiyonunu döndürür. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | Belirtilen tarih ve saatten başlayarak bir sonraki çalışma zamanının başlangıcını hesaplar. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Belirtilen günün takvime göre bir çalışma günü olup olmadığını belirler. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | Takvimin tanımlı çalışma saatlerine sahip olup olmadığını döndürür. |

## Örnekler

Atamanın takviminde hesaplama yapmak için Calendar.GetIntersectionCalendar() metodunun nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

foreach (var ra in project.ResourceAssignments)
{
    if (ra.Resource == null)
    {
        continue;
    }

    ICalendar assignmentCalendar;

    Calendar taskCalendar = ra.Task.Calendar != null && !ra.Task.Duration.IsEstimated ? ra.Task.Calendar : null;
    Calendar resourceCalendar = ra.Resource.Calendar != null && !ra.Task.IgnoreResourceCalendar
        ? ra.Resource.Calendar
        : null;

    if (taskCalendar != null && resourceCalendar != null && !ReferenceEquals(taskCalendar, resourceCalendar))
    {
        assignmentCalendar = Calendar.GetIntersectionCalendar(taskCalendar, resourceCalendar);
    }
    else
    {
        assignmentCalendar = taskCalendar ?? resourceCalendar;
    }

    if (assignmentCalendar == null)
    {
        assignmentCalendar = project.Calendar;
    }

    var workingHours = assignmentCalendar.GetWorkingHours(ra.Start, ra.Finish);

    Console.WriteLine("Working hours for assignment '{0}' : {1}", ra, workingHours);

    var date = new DateTime(2025, 4, 7);
    Console.WriteLine("Working times for date '{0}':", date);

    foreach (var wt in assignmentCalendar.GetWorkingTimes(date))
    {
        Console.WriteLine("{0} - {1}", wt.From.TimeOfDay, wt.To.TimeOfDay);
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


