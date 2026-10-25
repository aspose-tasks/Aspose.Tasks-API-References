---
title: "클래스 WeekDayCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WeekDayCollection 클래스. WeekDay 객체의 컬렉션을 나타냅니다"
type: docs
weight: 3550
url: /ko/net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

[`WeekDay`](../weekday/) 객체의 컬렉션을 나타냅니다.

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | `WeekDayCollection` 객체에 포함된 객체 수를 가져옵니다. |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | 지정된 인덱스에서 항목 값을 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | 이 객체에 [`WeekDay`](../weekday/) 인스턴스를 추가합니다. |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | WeekDayCollection 객체를 정리합니다. |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | 컬렉션에 지정된 [`WeekDay`](../weekday/)이 포함되어 있는지 확인합니다. |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | 컬렉션 내용을 지정된 인덱스의 배열에 복사합니다. |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | 지정된 [`WeekDay`](../weekday/)의 인덱스를 반환합니다. |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | 지정된 인덱스에 [`WeekDay`](../weekday/)을 삽입합니다. |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | 존재한다면 지정된 [`WeekDay`](../weekday/)을 제거합니다. |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | 지정된 인덱스의 항목을 제거합니다. |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | WeekDayCollection 객체를 [`WeekDay`](../weekday/) 객체 목록으로 변환합니다. |

## 예제

주 요일을 정리합니다

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// 토요일 주 요일을 제거합니다
calendar.WeekDays.Clear();

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
var saturday = WeekDay.CreateDefaultWorkingDay(DayType.Saturday);
var sunday = WeekDay.CreateDefaultWorkingDay(DayType.Sunday);

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

var fridayWorkingTimes = new List<WorkingTime> { new WorkingTime(new DateTime(2020, 4, 13, 8, 0, 0), new DateTime(2020, 4, 13, 12, 0, 0)) };

var friday = new WeekDay(DayType.Friday, fridayWorkingTimes);
if (calendar.WeekDays.Contains(friday))
{
    calendar.WeekDays.Insert(4, friday);
}

Console.WriteLine("Calendar: " + calendar.Name);
Console.WriteLine("Week days count: " + calendar.WeekDays.Count);
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

// 일요일 주 요일을 제거합니다
calendar.WeekDays.RemoveAt(5);

// 주 요일을 복사합니다
if (calendar.WeekDays.IndexOf(saturday) > 0)
{
    calendar.WeekDays.Remove(sunday);
}

Console.WriteLine("Working times after weekend was removed: ");
List<WeekDay> weekDays = calendar.WeekDays.ToList();
foreach (var day in weekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

var hour24Calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(hour24Calendar);

// 클래스 PrimaveraProjectProperties
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### 또 보기

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


