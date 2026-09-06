---
title: "Calendar.WorkWeeks"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Calendar. يحصل على كائن WorkWeekCollections. مجموعة أسابيع العمل المرتبطة بالتقويم"
type: docs
weight: 130
url: /ar/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

يحصل على كائن WorkWeekCollections. مجموعة أسابيع العمل المرتبطة بالتقويم.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## الأمثلة

يوضح كيفية قراءة معلومات أسبوع العمل.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // عرض اسم أسبوع العمل، من وإلى التواريخ
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // هذه البيانات تتعلق بالكامل بزر \"Details.\" يمكنك تعيين أوقات عمل خاصة ليوم أسبوع خاص أو حتى جعله غير عامل
    foreach (var day in workWeek.WeekDays)
    {
        // يمكنك أيضًا التنقل عبر أوقات العمل وعرضها
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### انظر أيضًا

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


