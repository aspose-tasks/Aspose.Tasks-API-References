---
title: "Calendar.Make24HourCalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 지정된 Calendar를 24시간 캘린더로 만듭니다. 24시간 캘린더는 주의 모든 요일이 연중무휴로 작업하는 캘린더입니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

주어진 Calendar를 24시간 캘린더로 만듭니다. 24시간 캘린더는 주의 모든 날이 24시간 연속 근무하는 캘린더입니다.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 캘린더 | Calendar | Calendar를 사용하여 24시간 캘린더를 만듭니다. |

### 반환 값

24시간 캘린더.

## 예제

24시간 캘린더를 만드는 방법을 보여줍니다.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24시간이 출력됩니다.
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

새 캘린더를 24시간 캘린더로 변환하는 방법을 보여줍니다.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24시간이 출력됩니다.
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


