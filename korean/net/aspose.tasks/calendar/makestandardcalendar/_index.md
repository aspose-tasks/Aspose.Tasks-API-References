---
title: "Calendar.MakeStandardCalendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 메서드. 기본 표준 캘린더를 생성합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

기본 표준 캘린더를 생성합니다.

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 캘린더 | Calendar | 표준 캘린더를 만들기 위한 Calendar |

### 반환 값

월요일부터 금요일까지 5근무일이며 근무 시간은 8-12시와 13-17시인 캘린더.

## 예제

표준 캘린더를 만드는 방법을 보여줍니다.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// 작업 시간 표시
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

예외일이 포함된 캘린더를 만드는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// 캘린더 정보를 업데이트합니다
Calendar.MakeStandardCalendar(calendar);
calendar.Name = "Test calendar";
var exception = new CalendarException();
exception.Name = "Exception 1";
exception.FromDate = DateTime.Now;
exception.ToDate = DateTime.Now.AddDays(2);
exception.DayWorking = true;

exception.WorkingTimes.Add(new WorkingTime(9, 13));
exception.WorkingTimes.Add(new WorkingTime(14, 19));
exception.WorkingTimes.Add(new WorkingTime(20, 21));
calendar.Exceptions.Add(exception);

var exception2 = new CalendarException();
exception.Name = "Exception 2";
exception2.FromDate = DateTime.Now.AddDays(7);
exception2.ToDate = exception2.FromDate;
exception2.DayWorking = false;
calendar.Exceptions.Add(exception2);

project.Set(Prj.Calendar, calendar);

project.Save(OutDir + "WriteUpdatedCalendarDataToMPP_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


