---
title: "Calendar.WeekDays"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Calendar 속성. 이 캘린더에 대한 WeekDaysCollection을 가져옵니다. 캘린더를 정의하는 요일 컬렉션입니다."
type: docs
weight: 120
url: /ko/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

이 캘린더에 대한 WeekDaysCollection을 가져옵니다. 캘린더를 정의하는 평일 컬렉션입니다.

```csharp
public WeekDayCollection WeekDays { get; }
```

## 예제

새 캘린더를 정의하고, 요일을 추가하며, 각 요일에 대한 작업 시간을 정의하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 캘린더 정의
var calendar = project.Calendars.Add("Calendar1");

// 월요일부터 목요일까지 기본 시간표로 작업일을 추가합니다.
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// 금요일을 짧은 작업일로 설정합니다.
var weekDay = new WeekDay(DayType.Friday);

// 작업 시간을 설정합니다. DateTime의 시간 부분만 중요합니다.
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// 프로젝트 작업 중...
```

### 또 보기

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


