---
title: "클래스 WorkWeekCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WorkWeekCollection 클래스. WorkWeek 객체의 컬렉션을 나타냅니다."
type: docs
weight: 3650
url: /ko/net/aspose.tasks/workweekcollection/
---
## WorkWeekCollection class

[`WorkWeek`](../workweek/) 객체의 컬렉션을 나타냅니다.

```csharp
public class WorkWeekCollection : IList<WorkWeek>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/workweekcollection/count/) { get; } | 이 `WorkWeekCollection` 객체에 포함된 객체 수를 가져옵니다. |
| [Item](../../aspose.tasks/workweekcollection/item/) { get; set; } | 지정된 인덱스의 요소를 반환합니다. |
| [ParentCalendar](../../aspose.tasks/workweekcollection/parentcalendar/) { get; } | 상위 캘린더를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/workweekcollection/add/)(WorkWeek) | 이 컬렉션 객체에 WorkWeek 인스턴스를 추가합니다. |
| [GetEnumerator](../../aspose.tasks/workweekcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [ToList](../../aspose.tasks/workweekcollection/tolist/)() | `WorkWeekCollection` 객체를 [`WorkWeek`](../workweek/) 객체 목록으로 변환합니다. |

## 예제

캘린더에 대한 사용자 정의 작업 주를 만드는 방법을 보여줍니다.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // 작업 주 이름, 상위 캘린더 이름, 시작 및 종료 날짜를 표시합니다
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // 이 데이터는 "Details." 버튼과 관련된 것으로, 특정 요일에 특수 작업 시간을 설정하거나 비작업으로 만들 수 있습니다.
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // 작업 시간을 추가로 탐색하고 이를 표시할 수 있습니다.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### 또 보기

* class [WorkWeek](../workweek/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


