---
title: "Aspose::Tasks::Calendar 클래스"
linktitle: "캘린더"
articleTitle: "캘린더"
second_title: "C++용 Aspose.Tasks"
description: "프로젝트에서 사용되는 달력을 나타냅니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

프로젝트에서 사용되는 달력을 나타냅니다.

처음부터 간단한 캘린더를 만드는 방법.

```cpp
[C#]
// 빈 캘린더 만들기
Calendar calendar = new Calendar("New calendar");
// 기본 근무일을 추가합니다 (9:00부터 17:00까지 8시간 근무).
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// 새 작업일 만들기
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
// 주말을 추가합니다
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```cpp
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

캘린더는 표준 근무 및 비근무 시간을 정의하는 데 사용됩니다. 프로젝트에는 하나의 기본 캘린더가 있어야 합니다. 작업 및 리소스는 기본 캘린더를 기반으로 하는 자체 비기본 캘린더를 가질 수 있습니다.

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Delete](./delete/) | 프로젝트에서 캘린더를 제거합니다. |
| [Equals](./equals/) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [get_BaseCalendar](./get_basecalendar/) | 이 캘린더가 의존하는 기본 캘린더를 가져옵니다. 캘린더가 기본 캘린더가 아닌 경우에만 적용됩니다. |
| [get_Exceptions](./get_exceptions/) | CalendarExceptionCollection 객체를 가져옵니다. 캘린더와 연결된 예외 컬렉션입니다. |
| [get_Guid](./get_guid/) | 캘린더의 Guid를 가져옵니다. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | 캘린더가 기본 캘린더인지 여부를 나타내는 값을 가져옵니다. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | 캘린더가 기준 캘린더인지 여부를 나타내는 값을 가져옵니다. |
| [get_Name](./get_name/) | 캘린더의 이름을 가져옵니다. |
| [get_Uid](./get_uid/) | 캘린더의 고유 식별자를 가져옵니다. |
| [get_WeekDays](./get_weekdays/) | 이 캘린더에 대한 WeekDaysCollection을 가져옵니다. 캘린더를 정의하는 요일 컬렉션입니다. |
| [get_WorkWeeks](./get_workweeks/) | WorkWeekCollections 객체를 가져옵니다. 캘린더와 연결된 작업 주 컬렉션입니다. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | 캘린더에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| [GetHashCode](./gethashcode/) | 클래스 인스턴스에 대한 해시 코드를 반환합니다. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | 두 캘린더의 작업 일정 교차점에 대한 계산을 수행하는 데 사용할 수 있는 ICalendar 인스턴스를 가져옵니다. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | 지정된 날짜에 대한 다음 작업일 시작 시간을 계산합니다. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | 지정된 날짜로부터 이전 작업일의 종료 시간을 계산합니다. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | 지정된 종료 날짜와 기간을 기반으로 시작 날짜를 반환합니다. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | 작업의 시작 날짜, 분할 부분 및 작업 기간을 기반으로 작업 종료 날짜와 시간을 계산합니다. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | 지정된 날짜의 작업 시간을 반환합니다. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | 지정된 날짜들 사이의 작업 시간을 반환합니다. |
| [GetWorkingTimes](./getworkingtimes/) | 지정된 날짜에 대한 WorkingTimeCollection을 반환합니다. |
| [GetWorkStart](./getworkstart/) | 지정된 날짜와 시간부터 시작되는 다음 작업 시간 시작을 계산합니다. |
| [IsDayWorking](./isdayworking/) | 캘린더에 따라 지정된 날이 작업일인지 여부를 판단합니다. |
| [IsEmpty](./isempty/) | 캘린더에 근무 시간이 정의되지 않았는지 여부를 반환합니다. |
| [Make24HourCalendar](./make24hourcalendar/) | 지정된 캘린더를 24시간 캘린더로 만듭니다. 24시간 캘린더는 주의 모든 요일이 24시간 연속 근무하는 캘린더입니다. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | 지정된 캘린더를 야간 근무 캘린더로 만듭니다. |
| [MakeStandardCalendar](./makestandardcalendar/) | 기본 표준 캘린더를 생성합니다. |
| [set_BaseCalendar](./set_basecalendar/) | 이 캘린더가 의존하는 기본 캘린더를 설정합니다. 캘린더가 기본 캘린더가 아닌 경우에만 적용됩니다. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | 캘린더가 기준 캘린더인지 여부를 나타내는 값을 설정합니다. |
| [set_Name](./set_name/) | 캘린더의 이름을 설정합니다. |
| [set_Uid](./set_uid/) | 캘린더의 고유 식별자를 설정합니다. |

