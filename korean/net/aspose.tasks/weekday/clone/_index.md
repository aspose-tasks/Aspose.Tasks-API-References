---
title: "WeekDay.Clone"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WeekDay 메서드. 주중의 깊은 복사본을 반환합니다"
type: docs
weight: 80
url: /ko/net/aspose.tasks/weekday/clone/
---
## WeekDay.Clone method

요일의 깊은 복사본을 반환합니다.

```csharp
public WeekDay Clone()
```

### 반환 값

주중의 깊은 복사본을 반환합니다.

## 예제

주중을 복제하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var calendar = project.Calendars.GetByUid(1);
var weekDay1 = calendar.WeekDays[0];

// 주중의 깊은 복사본을 생성합니다
var weekDay2 = weekDay1.Clone();

// 캘린더의 동일성은 weekday의 속성과 비교됩니다:
// weekday.DayType
// weekday.DayWorking
// weekday.FromDate
// weekday.ToDate
// weekday.WorkingTimes
Console.WriteLine("WeekDay 1 Day Type: " + weekDay1.DayType);
Console.WriteLine("WeekDay 1 Day Working: " + weekDay1.DayWorking);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.FromDate);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.ToDate);
Console.WriteLine("WeekDay 1 WorkingTimes: " + weekDay1.WorkingTimes);
Console.WriteLine("WeekDay 2 Day Type: " + weekDay2.DayType);
Console.WriteLine("WeekDay 2 Day Working: " + weekDay2.DayWorking);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.FromDate);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.ToDate);
Console.WriteLine("WeekDay 2 WorkingTimes: " + weekDay2.WorkingTimes);
Console.WriteLine("Are weekdays equal: " + weekDay1.Equals(weekDay2));
Console.WriteLine("Are weekdays equal (by reference): " + ReferenceEquals(weekDay1, weekDay2));
```

### 또 보기

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


