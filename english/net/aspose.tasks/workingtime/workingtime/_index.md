---
title: WorkingTime.WorkingTime
second_title: Aspose.Tasks for .NET API Reference
description: WorkingTime constructor. Initializes a new instance of the WorkingTime class with a interval with the specified start and finish times
type: docs
weight: 10
url: /net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Initializes a new instance of the [`WorkingTime`](../) class with a interval with the specified start and finish times.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | DateTime | interval start time |
| toTime | DateTime | interval end time |

## Examples

Shows how to work with working time information.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // This data is all about "Details." button you can set special working times for special WeekDay or even make it nonworking
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // You can further traverse through working times and display these
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### See Also

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Initializes a new instance of the [`WorkingTime`](../) class with an interval item with the specified start and finish times.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | TimeSpan | Interval's start time represented by TimeSpan struct. |
| toTime | TimeSpan | Interval's end time represented by TimeSpan struct. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | When toTime less than of equal to toTime argument or when interval between fromTime and toTime is greater than 24 hours. |

## Examples

The overload of WorkingTime ctor can be used to initialize interval's start and end using TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### See Also

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Initializes a new instance of the [`WorkingTime`](../) class with an interval item with the specified start and finish times.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fromHours | Int32 | Interval's start time represented by whole number of hours (0-24). |
| toHours | Int32 | Interval's end time represented by whole number of hours (0-24). |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | When toTime less than of equal to toTime argument or when interval between fromTime and toTime is greater than 24 hours. |

## Examples

The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

Shows how to check working time equality.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// the equality of calendars is checked against to working time's from and to dates.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### See Also

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


