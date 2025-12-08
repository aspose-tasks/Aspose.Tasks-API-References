---
title: Calendar.WorkWeeks
second_title: Aspose.Tasks for .NET API Reference
description: Calendar property. Gets WorkWeekCollections object. The collection of work weeks that is associated with the calendar
type: docs
weight: 130
url: /net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

Gets WorkWeekCollections object. The collection of work weeks that is associated with the calendar.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## Examples

Shows how to read work week information.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // Display work week name, from and to dates
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // This data is all about "Details." button you can set special working times for special WeekDay or even make it nonworking
    foreach (var day in workWeek.WeekDays)
    {
        // You can further traverse through working times and display these
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### See Also

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


