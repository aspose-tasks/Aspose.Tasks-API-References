---
title: "WorkingTimeCollection 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WorkingTimeCollection 클래스. WorkingTimeCollection 객체의 컬렉션을 나타냅니다"
type: docs
weight: 3670
url: /ko/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

`WorkingTimeCollection` 객체의 컬렉션을 나타냅니다.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | 이 `WorkingTimeCollection` 객체에 포함된 객체 수를 가져옵니다. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | 지정된 인덱스의 요소를 반환합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | 새 WorkingTime 인스턴스를 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | 컬렉션에서 모든 [`WorkingTime`](../workingtime/) 항목을 제거합니다. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | 지정된 요소가 List에 있는지 확인합니다. 선형 O(n) 검색을 수행합니다. |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | 특정 인덱스에서 시작하여 컬렉션 내용을 Array에 복사합니다. |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | 이 컬렉션에서 [`WorkingTime`](../workingtime/) 인스턴스를 제거합니다. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | WorkingTimeCollection 객체를 [`WorkingTime`](../workingtime/) 객체 목록으로 변환합니다. |

## 예제

작업 시간 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// Saturday의 작업 시간을 출력합니다
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// sunday의 작업 시간을 출력합니다
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // 작업 시간을 추가로 탐색하고 이를 표시할 수 있습니다.
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### 또 보기

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


