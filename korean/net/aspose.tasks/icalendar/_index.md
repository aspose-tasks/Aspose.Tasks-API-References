---
title: "인터페이스 ICalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ICalendar 인터페이스. 날짜와 기간의 다양한 계산에 사용할 수 있는 캘린더 추상화를 나타냅니다."
type: docs
weight: 840
url: /ko/net/aspose.tasks/icalendar/
---
## ICalendar interface

날짜 및 기간의 다양한 계산에 사용할 수 있는 캘린더 추상화를 나타냅니다.

```csharp
public interface ICalendar
```

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | 캘린더에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | 캘린더에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | 지정된 날짜에 대한 다음 작업일 시작 시간을 계산합니다. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | 지정된 날짜로부터 이전 작업일의 종료 시간을 계산합니다. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | 지정된 종료 날짜와 기간을 기반으로 시작 날짜를 반환합니다. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | 지정된 종료 날짜와 기간을 기반으로 시작 날짜를 반환합니다. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | 작업의 시작 날짜, 분할 부분 및 작업 기간을 기준으로 작업 종료 날짜와 시간을 계산합니다. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | 지정된 날짜의 작업 시간 양을 반환합니다. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | WorkUnit을 반환합니다 - 지정된 날짜 시간 구간에 대한 작업 시간의 시작, 종료 및 기간. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | 지정된 날짜 사이의 작업 시간 양을 반환합니다. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | 지정된 날짜에 대한 작업 시간의 [`WorkingTimeCollection`](../workingtimecollection/)을 반환합니다. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | 지정된 날짜와 시간부터 시작되는 다음 작업 시간 시작을 계산합니다. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | 캘린더에 따라 지정된 날짜가 작업일인지 여부를 판단합니다. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | 캘린더에 작업 시간이 정의되어 있지 않은지 여부를 반환합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


