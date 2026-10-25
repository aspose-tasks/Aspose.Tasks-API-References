---
title: "클래스 DailyCalendarRepetition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.DailyCalendarRepetition 클래스. 캘린더 일자를 기반으로 한 일일 반복 패턴의 반복을 위한 클래스를 나타냅니다."
type: docs
weight: 390
url: /ko/net/aspose.tasks/dailycalendarrepetition/
---
## DailyCalendarRepetition class

달력 일자를 기반으로 하는 일일 반복 패턴의 반복을 위한 클래스를 나타냅니다.

```csharp
public class DailyCalendarRepetition : DailyRepetitionBase
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [DailyCalendarRepetition](dailycalendarrepetition/)() | 새 `DailyCalendarRepetition` 클래스의 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | 발생 간의 일 수 간격을 나타내는 일 수를 가져오거나 설정합니다. |

## 예제

반복 작업을 생성하는 동안 일일 작업 반복 패턴 반복 및 '24시간'을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(calendar);
var parameters = new RecurringTaskParameters
{
    TaskName = "t1",
    Duration = project.GetDuration(1, TimeUnitType.Day),
    RecurrencePattern = new DailyRecurrencePattern
    {
        Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
        RecurrenceRange = new EndByRecurrenceRange
        {
            Start = new DateTime(2018, 7, 2, 0, 0, 0),
            Finish = new DateTime(2018, 7, 8, 16, 0, 0)
        }
    }
};
parameters.SetCalendar(project, "24 Hours");
project.RootTask.Children.Add(parameters);

// 프로젝트를 계속 작업합니다...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


