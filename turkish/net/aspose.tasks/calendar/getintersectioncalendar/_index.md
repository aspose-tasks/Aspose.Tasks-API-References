---
title: "Calendar.GetIntersectionCalendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. 2 takvimin çalışma programlarının kesişimi üzerinde hesaplamalar yapmak için kullanılabilecek ICalendar örneğini alır"
type: docs
weight: 280
url: /tr/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

[`ICalendar`](../../icalendar/) örneğini alır; bu örnek 2 takvimin çalışma programlarının kesişimi üzerinde hesaplamalar yapmak için kullanılabilir.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| calendar1 | Takvim | İlk takvim. |
| calendar2 | Takvim | İkinci takvim. |

### Dönüş Değeri

ICalendar arayüzünün uygulanması.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | Argümanlardan biri null olduğunda. |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


