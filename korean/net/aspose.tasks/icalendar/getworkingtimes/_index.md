---
title: "ICalendar.GetWorkingTimes"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ICalendar 메서드. 지정된 날짜에 대한 작업 시간의 WorkingTimeCollection을 반환합니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

지정된 날짜에 대한 작업 시간의 [`WorkingTimeCollection`](../../workingtimecollection/)을 반환합니다.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dt | DateTime | 작업 시간을 가져올 날짜. |

### 반환 값

[`WorkingTime`](../../workingtime/) 인스턴스의 컬렉션.

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


