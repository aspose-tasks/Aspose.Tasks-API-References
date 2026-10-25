---
title: "Calendar.WorkWeeks"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar özelliği. WorkWeekCollections nesnesini alır. Takvimle ilişkili çalışma haftalarının koleksiyonu"
type: docs
weight: 130
url: /tr/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

WorkWeekCollections nesnesini alır. Takvimle ilişkili çalışma haftalarının koleksiyonunu içerir.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## Örnekler

Çalışma haftası bilgilerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // Çalışma haftası adını, başlangıç ve bitiş tarihlerini göster
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // Bu veri, "Details." düğmesiyle ilgilidir; özel bir Hafta Günü için özel çalışma zamanları ayarlayabilir veya hatta çalışmaz olarak işaretleyebilirsiniz.
    foreach (var day in workWeek.WeekDays)
    {
        // Çalışma zamanları arasında daha fazla dolaşabilir ve bunları görüntüleyebilirsiniz.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


