---
title: "클래스 Calendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Calendar 클래스. 프로젝트에서 사용되는 캘린더를 나타냅니다."
type: docs
weight: 230
url: /ko/net/aspose.tasks/calendar/
---
## Calendar class

프로젝트에서 사용되는 캘린더를 나타냅니다.

```csharp
public class Calendar : ICalendar
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | 이 캘린더가 의존하는 기본 캘린더를 가져오거나 설정합니다. 캘린더가 기본 캘린더가 아닌 경우에만 적용됩니다. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | CalendarExceptionCollection 객체를 가져옵니다. 캘린더와 연결된 예외 컬렉션입니다. |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | 캘린더의 Guid를 가져옵니다. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | 캘린더가 기본 캘린더인지 여부를 나타내는 값을 가져옵니다. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | 캘린더가 기준선 캘린더인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | 캘린더의 이름을 가져오거나 설정합니다. |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | Primavera 형식에서 읽은 캘린더에 대한 Primavera 전용 속성을 포함하는 객체를 가져옵니다. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | 캘린더의 고유 식별자를 가져오거나 설정합니다. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | 이 캘린더에 대한 WeekDaysCollection을 가져옵니다. 캘린더를 정의하는 평일 컬렉션입니다. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | WorkWeekCollections 객체를 가져옵니다. 캘린더와 연결된 작업 주 컬렉션입니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | 주어진 Calendar를 24시간 캘린더로 만듭니다. 24시간 캘린더는 주의 모든 날이 24시간 연속 근무하는 캘린더입니다. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | 주어진 캘린더를 야간 근무 캘린더로 만듭니다. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | 기본 표준 캘린더를 생성합니다. |
| [Delete](../../aspose.tasks/calendar/delete/)() | 프로젝트에서 캘린더를 제거합니다. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | 캘린더에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | 캘린더에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | 클래스 인스턴스에 대한 해시 코드를 반환합니다. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | 지정된 날짜에 대한 다음 작업일 시작 시간을 계산합니다. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | 지정된 날짜로부터 이전 작업일의 종료 시간을 계산합니다. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | 지정된 종료 날짜와 기간을 기반으로 시작 날짜를 반환합니다. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | 지정된 종료 날짜와 기간을 기반으로 시작 날짜를 반환합니다. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | 작업의 시작 날짜, 분할 부분 및 작업 기간을 기준으로 작업 종료 날짜와 시간을 계산합니다. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | 지정된 날짜의 작업 시간 양을 반환합니다. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | 지정된 날짜 시간 구간에 대한 작업 단위 - 시작, 종료 및 작업 시간 지속 시간을 반환합니다. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | 지정된 날짜 사이의 작업 시간 양을 반환합니다. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | 지정된 날짜에 대한 작업 시간의 [`WorkingTimeCollection`](../workingtimecollection/)을 반환합니다. |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | 지정된 날짜와 시간부터 시작되는 다음 작업 시간 시작을 계산합니다. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | 캘린더에 따라 지정된 날짜가 작업일인지 여부를 판단합니다. |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | 캘린더에 작업 시간이 정의되어 있지 않은지 여부를 반환합니다. |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | 2개의 캘린더 작업 일정 교차점에 대한 계산을 수행하는 데 사용할 수 있는 [`ICalendar`](../icalendar/) 인스턴스를 가져옵니다. |

## 비고

캘린더는 표준 근무 및 비근무 시간을 정의하는 데 사용됩니다. 프로젝트에는 하나의 기본 캘린더가 있어야 합니다. 작업 및 리소스는 기본 캘린더를 기반으로 하는 자체 비기본 캘린더를 가질 수 있습니다.

## 예제

처음부터 간단한 캘린더를 만드는 방법.

```csharp
[C#]
// 빈 캘린더 생성
Calendar calendar = new Calendar("New calendar");
// 기본 근무일을 추가합니다 (9:00부터 17:00까지 8시간 근무).
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// 새 작업일 생성
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
// 주말을 추가합니다.
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
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
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

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

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


