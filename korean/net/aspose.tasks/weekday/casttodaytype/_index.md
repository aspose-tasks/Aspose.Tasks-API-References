---
title: "WeekDay.CastToDayType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WeekDay 메서드. .Nets DayOfWeek를 DayType으로 변환합니다"
type: docs
weight: 120
url: /ko/net/aspose.tasks/weekday/casttodaytype/
---
## WeekDay.CastToDayType method

.Net의 DayOfWeek를 [`DayType`](../daytype/)으로 변환합니다.

```csharp
public static DayType CastToDayType(DayOfWeek dw)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dw | DayOfWeek | 변환할 요일. |

### 반환 값

변환된 요일 유형.

## 예제

요일을 정의하여 새 캘린더를 만드는 방법을 보여줍니다.

```csharp
var project = new Project();

// 캘린더 정의
var calendar = project.Calendars.Add("Calendar1");

// 월요일부터 목요일까지 기본 시간표로 작업일을 추가합니다.
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// 예외 일자의 시작 및 종료 날짜를 확인합니다
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// 금요일을 짧은 작업일로 설정합니다.

// 작업 시간을 설정합니다. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// <see cref=\"DayOfWeek\" />를 <see cref=\"Aspose.Tasks.DayType\" />로 변환하는 방법이 있습니다.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

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

* enum [DayType](../../daytype/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


