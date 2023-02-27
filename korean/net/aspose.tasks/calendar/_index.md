---
title: Calendar
second_title: .NET API 참조용 Aspose.Tasks
description: 프로젝트에서 사용하는 달력을 나타냅니다.
type: docs
weight: 230
url: /ko/net/aspose.tasks/calendar/
---
## Calendar class

프로젝트에서 사용하는 달력을 나타냅니다.

```csharp
public class Calendar
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | 이 달력이 종속된 기본 달력을 가져오거나 설정합니다. 달력이 기본 달력이 아닌 경우에만 적용됩니다. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | CalendarExceptionCollection 개체를 가져옵니다. 달력과 관련된 예외 컬렉션입니다. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | 달력이 기본 달력인지 여부를 나타내는 값을 가져옵니다. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | 달력이 기준 달력인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | 달력의 이름을 가져오거나 설정합니다. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | 달력의 고유 식별자를 가져오거나 설정합니다. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | 이 달력에 대한 WeekDaysCollection을 가져옵니다. 달력을 정의하는 요일 모음입니다. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | WorkWeekCollections 개체를 가져옵니다. 달력과 연결된 작업 주의 모음입니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | 주어진 달력을 24시간 달력으로 만듭니다. 24시간 달력은 매일 24시간 근무하는 달력입니다. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | 주어진 달력을 야간 근무 달력으로 만듭니다. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | 기본 표준 달력을 생성합니다. |
| [Delete](../../aspose.tasks/calendar/delete/)() | 프로젝트에서 캘린더를 제거합니다. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | 이 인스턴스가 지정된 개체와 같은지 여부를 나타내는 값을 반환합니다. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | 달력에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | 달력에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | 클래스의 인스턴스에 대한 해시 코드를 반환합니다. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | 날짜를 기준으로 다음 근무일을 계산합니다. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | 지정된 날짜로부터 이전 근무일 종료를 계산합니다. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | 지정된 FinishDate 및 기간을 기준으로 StartDate를 반환합니다. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | 지정된 FinishDate 및 기간을 기준으로 StartDate를 반환합니다. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | 시작 날짜, 분할 부분 및 기간에서 작업 완료 날짜 및 시간을 계산합니다. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | 날짜의 근무 시간을 반환합니다. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | 지정된 날짜의 근무 시간을 반환합니다. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | 반환[`WorkingTimeCollection`](../workingtimecollection/) 지정된 날짜의 작업 시간. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | 요일이 작업일인지 여부를 결정합니다. |

### 비고

달력은 표준 작업 시간과 휴무 시간을 정의하는 데 사용됩니다. 프로젝트에는 하나의 기본 달력이 있어야 합니다. 작업 및 리소스는 기본 캘린더를 기반으로 하는 고유한 비기본 캘린더를 가질 수 있습니다. .

### 예

처음부터 간단한 달력을 만드는 방법.

```csharp
[C#]
// 빈 캘린더 생성
Calendar calendar = new Calendar("New calendar");
// 기본 근무일 추가(9:00부터 17:00까지 8시간 근무)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// 새로운 근무일 생성
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// 작업 시간을 설정합니다. DateTime의 시간 부분만 중요합니다.
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// 주말 추가
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' 빈 캘린더 만들기
Dim calendar As Calendar =  New Calendar("New calendar")
' 기본 근무일 추가(9시부터 17시까지 8시간 근무)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' 새로운 새로운 근무일 만들기
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' 작업 시간을 설정합니다. DateTime의 시간 부분만 중요합니다.
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' 주말 추가
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### 또한보십시오

* 네임스페이스 [Aspose.Tasks](../../aspose.tasks/)
* 집회 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
