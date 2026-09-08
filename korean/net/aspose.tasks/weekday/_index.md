---
title: "클래스 WeekDay"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WeekDay 클래스. 주중의 일반 요일 또는 캘린더의 예외 일자를 정의하는 요일을 나타냅니다."
type: docs
weight: 3540
url: /ko/net/aspose.tasks/weekday/
---
## WeekDay class

요일을 기반으로 하는 패턴을 나타냅니다.

```csharp
public class WeekDay
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [WeekDay](weekday/#constructor)() | `WeekDay` 클래스의 새 인스턴스를 초기화합니다. |
| [WeekDay](weekday/#constructor_1)(DayType) | 지정된 day type으로 `WeekDay` 클래스의 새 인스턴스를 초기화합니다. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | 지정된 day type 및 작업 시간 기간 목록으로 `WeekDay` 클래스의 새 인스턴스를 초기화합니다. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | 지정된 day type 및 작업 시간 기간으로 `WeekDay` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | 날의 유형을 가져옵니다. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | 지정된 날짜 또는 day type이 작업일인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | 예외 시간의 시작을 가져오거나 설정합니다. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | 예외 시간의 끝을 가져오거나 설정합니다. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | 이 WeekDay 인스턴스에 대한 WorkingTimeCollection을 가져옵니다. 평일에 작업한 시간을 정의하는 작업 시간 컬렉션입니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | 기본 작업일을 생성합니다. |
| [Clone](../../aspose.tasks/weekday/clone/)() | 요일의 깊은 복사본을 반환합니다. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | `WeekDay` 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | 요일에 대한 작업 시간을 반환합니다. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | .Net의 DayOfWeek를 [`DayType`](./daytype/)으로 캐스팅합니다. |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | 지정된 요일에 대한 기본 시간 기간을 설정합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


