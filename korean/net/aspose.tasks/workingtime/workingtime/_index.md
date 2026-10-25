---
title: "WorkingTime.WorkingTime"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WorkingTime 생성자. 지정된 시작 및 종료 시간을 가진 인터벌로 WorkingTime 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

`[`WorkingTime`](../)` 클래스의 새 인스턴스를 지정된 시작 및 종료 시간을 가진 인터벌로 초기화합니다.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fromTime | DateTime | 인터벌 시작 시간 |
| toTime | DateTime | 인터벌 종료 시간 |

## 예제

작업 시간 정보를 사용하는 방법을 보여줍니다.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // 이 데이터는 "Details." 버튼과 관련된 것으로, 특정 요일에 특수 작업 시간을 설정하거나 비작업으로 만들 수 있습니다.
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
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
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### 또 보기

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

`[`WorkingTime`](../)` 클래스의 새 인스턴스를 지정된 시작 및 종료 시간을 가진 인터벌 항목으로 초기화합니다.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fromTime | TimeSpan | TimeSpan 구조체로 표현된 인터벌의 시작 시간. |
| toTime | TimeSpan | TimeSpan 구조체로 표현된 인터벌의 종료 시간. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | toTime이 toTime 인수보다 작거나 같을 때 또는 fromTime과 toTime 사이의 간격이 24시간을 초과할 때. |

## 예제

WorkingTime 생성자의 오버로드를 사용하여 TimeSpan을 이용해 구간의 시작과 끝을 초기화할 수 있습니다:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### 또 보기

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

`[`WorkingTime`](../)` 클래스의 새 인스턴스를 지정된 시작 및 종료 시간을 가진 인터벌 항목으로 초기화합니다.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fromHours | Int32 | 구간 시작 시간은 정수 시간(0-24)으로 표시됩니다. |
| toHours | Int32 | 구간 종료 시간은 정수 시간(0-24)으로 표시됩니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | toTime이 toTime 인수보다 작거나 같을 때 또는 fromTime과 toTime 사이의 간격이 24시간을 초과할 때. |

## 예제

WorkingTime 생성자의 오버로드를 사용하여 정수 시간으로 구간의 시작과 끝을 초기화할 수 있습니다:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

작업 시간 동일성을 확인하는 방법을 보여줍니다.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// 달력의 동일성은 작업 시간의 시작 및 종료 날짜와 비교하여 확인됩니다.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### 또 보기

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


