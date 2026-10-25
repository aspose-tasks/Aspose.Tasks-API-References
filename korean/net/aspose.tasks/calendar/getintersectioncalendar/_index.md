---
title: "Calendar.GetIntersectionCalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 두 캘린더의 작업 일정 교차점에 대한 계산을 수행하는 데 사용할 수 있는 ICalendar 인스턴스를 가져옵니다"
type: docs
weight: 280
url: /ko/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

두 캘린더의 작업 일정 교차점에 대한 계산을 수행하는 데 사용할 수 있는 [`ICalendar`](../../icalendar/) 인스턴스를 가져옵니다.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| calendar1 | Calendar | 첫 번째 캘린더. |
| calendar2 | Calendar | 두 번째 캘린더. |

### 반환 값

ICalendar 인터페이스 구현.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | 인수 중 하나가 null인 경우. |

## 예제

Calendar.GetIntersectionCalendar() 메서드를 사용하여 할당 캘린더에서 계산을 수행하는 방법을 보여줍니다.

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

### 또 보기

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


