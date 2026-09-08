---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 주어진 Calendar를 야간 근무 캘린더로 만듭니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

주어진 캘린더를 야간 근무 캘린더로 만듭니다.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 캘린더 | Calendar | Night Shift Calendar를 만들기 위한 Calendar. |

### 반환 값

Night Shift Calendar.

## 예제

야간 근무 캘린더를 만드는 방법을 보여줍니다.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// 작업 시간 표시
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

캘린더를 야간 근무 캘린더로 변환하는 방법을 보여줍니다.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// 작업 시간 표시
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


