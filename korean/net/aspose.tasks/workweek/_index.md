---
title: "클래스 WorkWeek"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WorkWeek 클래스. WorkWeek 클래스를 나타냅니다"
type: docs
weight: 3640
url: /ko/net/aspose.tasks/workweek/
---
## WorkWeek class

WorkWeek 클래스를 나타냅니다.

```csharp
public class WorkWeek
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [WorkWeek](workweek/)() | `WorkWeek` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [FromDate](../../aspose.tasks/workweek/fromdate/) { get; set; } | 작업 주의 시작 DateTime을 가져오거나 설정합니다 |
| [Name](../../aspose.tasks/workweek/name/) { get; set; } | 작업 주의 Name을 가져오거나 설정합니다 |
| [ToDate](../../aspose.tasks/workweek/todate/) { get; set; } | 작업 주의 종료 DateTime을 가져오거나 설정합니다 |
| [WeekDays](../../aspose.tasks/workweek/weekdays/) { get; } | 주 요일을 가져옵니다. |

## 예제

프로젝트에서 작업 주 정보를 읽는 방법을 보여줍니다.

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

Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


