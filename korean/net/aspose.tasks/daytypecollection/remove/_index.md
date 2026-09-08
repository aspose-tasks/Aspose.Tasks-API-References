---
title: "DayTypeCollection.Remove"
second_title: "Aspose.Tasks for .NET API 참조"
description: "DayTypeCollection 메서드. 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다."
type: docs
weight: 110
url: /ko/net/aspose.tasks/daytypecollection/remove/
---
## DayTypeCollection.Remove method

이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다.

```csharp
public bool Remove(DayType item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | DayType | 제거할 지정된 객체. |

### 반환 값

지정된 객체가 이 컬렉션에서 성공적으로 제거되면 true; 그렇지 않으면 false.

## 예제

주 요일 컬렉션을 사용하여 주간 캘린더 예외를 정의하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // "Exception 2"에서 일 유형을 일 유형으로 삭제합니다.
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// "Exception 2"에서 인덱스로 일 유형을 삭제합니다.
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// 예외를 변경합니다 (초기 프로젝트 데이터에 예외가 없습니다).
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// "Exception 3"에 대한 모든 요일을 제거합니다.
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### 또 보기

* enum [DayType](../../daytype/)
* class [DayTypeCollection](../)
* namespace [Aspose.Tasks](../../daytypecollection/)
* assembly [Aspose.Tasks](../../../)


