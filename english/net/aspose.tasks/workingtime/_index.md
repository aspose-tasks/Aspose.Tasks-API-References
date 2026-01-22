---
title: Class WorkingTime
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WorkingTime class. Represents a working time during a weekday
type: docs
weight: 3630
url: /net/aspose.tasks/workingtime/
---
## WorkingTime class

Represents a working time during a weekday.

```csharp
public class WorkingTime
```

## Constructors

| Name | Description |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | Initializes a new instance of the `WorkingTime` class with a interval with the specified start and finish times. |
| [WorkingTime](workingtime/#constructor)(int, int) | Initializes a new instance of the `WorkingTime` class with an interval item with the specified start and finish times. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | Initializes a new instance of the `WorkingTime` class with an interval item with the specified start and finish times. |

## Properties

| Name | Description |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | Gets the beginning of a working time. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | Gets the end of a working time. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | Checks that the objects are equal. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | Returns a hash code value for the instance of the `WorkingTime` class. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


