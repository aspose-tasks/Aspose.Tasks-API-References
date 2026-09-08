---
title: "클래스 WorkingTime"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WorkingTime 클래스. 평일 동안의 작업 시간을 나타냅니다."
type: docs
weight: 3660
url: /ko/net/aspose.tasks/workingtime/
---
## WorkingTime class

요일 중 작업 시간을 나타냅니다.

```csharp
public class WorkingTime
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | `WorkingTime` 클래스의 새 인스턴스를 지정된 시작 및 종료 시간으로 구간을 설정하여 초기화합니다. |
| [WorkingTime](workingtime/#constructor)(int, int) | `WorkingTime` 클래스의 새 인스턴스를 지정된 시작 및 종료 시간으로 구간 항목을 사용하여 초기화합니다. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | `WorkingTime` 클래스의 새 인스턴스를 지정된 시작 및 종료 시간으로 구간 항목을 사용하여 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | 작업 시간의 시작을 가져옵니다. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | 작업 시간의 끝을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | 객체가 동일한지 확인합니다. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | `WorkingTime` 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


