---
title: "ICalendar.GetWorkingTimes"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ICalendar yöntemi. Belirtilen tarih için çalışma zamanlarının WorkingTimeCollection'ını döndürür"
type: docs
weight: 80
url: /tr/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

Belirtilen tarih için çalışma zamanlarının [`WorkingTimeCollection`](../../workingtimecollection/) koleksiyonunu döndürür.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dt | DateTime | Çalışma saatlerini almak için tarih. |

### Dönüş Değeri

[`WorkingTime`](../../workingtime/) örneklerinin koleksiyonu.

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


