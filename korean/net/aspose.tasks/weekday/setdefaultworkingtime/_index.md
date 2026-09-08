---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WeekDay 메서드. 지정된 요일에 대한 기본 시간 기간을 설정합니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

지정된 요일에 대한 기본 시간 기간을 설정합니다.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| day | WeekDay | 기본 근무일을 설정할 요일입니다. |

## 예제

하루에 대한 기본 근무 시간을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 캘린더 정의
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// 월요일부터 목요일까지 기본 시간표로 작업일을 추가합니다.
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

// 모든 작업 시간을 출력합니다
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### 또 보기

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


