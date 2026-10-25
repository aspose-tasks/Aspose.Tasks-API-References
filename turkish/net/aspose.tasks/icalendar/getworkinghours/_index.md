---
title: "ICalendar.GetWorkingHours"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ICalendar yöntemi. Belirtilen tarih zaman aralığı için çalışma saatlerinin WorkUnit Başlangıç, Bitiş ve Süresini döndürür."
type: docs
weight: 60
url: /tr/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

WorkUnit - Belirtilen tarih zaman aralığı için çalışma saatlerinin Başlangıç, Bitiş ve Süresini döndürür.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Aralığın başlangıç tarihi. |
| bitiş | DateTime | Aralığın bitiş tarihi. |

### Dönüş Değeri

[`WorkUnit`](../../workunit/) sınıfının, çalışma saatlerinin Başlangıç, Bitiş ve Süresini içeren örneği.

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Belirtilen tarihteki çalışma saatlerinin miktarını döndürür.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dt | DateTime | Çalışma saatlerini almak için tarih. |

### Dönüş Değeri

Belirtilen tarihteki çalışma saatleri.

### Ayrıca Bakınız

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


