---
title: "Calendar"
second_title: "Aspose.Tasks for Python via .NET API 참조"
description: 
type: docs
weight: 140
url: /ko/python-net/aspose.tasks/calendar/
---

## Calendar class

프로젝트에서 사용되는 캘린더를 나타냅니다.

Calendar 유형은 다음 멤버를 노출합니다:
## 속성
| 이름 | 설명 |
| :- | :- |
| name | 캘린더의 이름을 가져오거나 설정합니다. |
| uid | 캘린더의 고유 식별자를 가져오거나 설정합니다. |
| week_days | 이 캘린더에 대한 WeekDaysCollection을 가져옵니다.<br/>            캘린더를 정의하는 평일 컬렉션입니다. |
| exceptions | CalendarExceptionCollection 객체를 가져옵니다.<br/>            캘린더와 연관된 예외 컬렉션입니다. |
| work_weeks | WorkWeekCollections 객체를 가져옵니다.<br/>            캘린더와 연관된 작업 주 컬렉션입니다. |
| is_base_calendar | 캘린더가 기본 캘린더인지 여부를 나타내는 값을 가져옵니다. |
| base_calendar | 이 캘린더가 의존하는 기본 캘린더를 가져오거나 설정합니다.<br/>            캘린더가 기본 캘린더가 아닌 경우에만 적용됩니다. |
| is_baseline_calendar | 캘린더가 기준 캘린더인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| guid | 캘린더의 Guid를 가져옵니다. |
| primavera_properties | Primavera 형식에서 읽은 캘린더에 대한 Primavera 전용 속성을 포함하는 객체를 가져옵니다. |
## 메서드
| 이름 | 설명 |
| :- | :- |
| get_start_date_from_finish_and_duration(finish, duration) | 지정된 종료 날짜와 기간을 기반으로 시작 날짜를 반환합니다. |
| get_start_date_from_finish_and_duration(finish, duration) | 지정된 종료 날짜와 기간을 기반으로 시작 날짜를 반환합니다. |
| get_working_hours(start, finish) | 지정된 날짜/시간 구간에 대한 작업 시간의 시작, 종료 및 기간을 나타내는 WorkUnit을 반환합니다. |
| get_working_hours(dt) | 지정된 날짜/시간 구간에 대한 작업 시간의 시작, 종료 및 기간을 나타내는 WorkUnit을 반환합니다. |
| get_finish_date_by_start_and_work(start, work) | 캘린더에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| get_finish_date_by_start_and_work(start, work) | 캘린더에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| get_intersection_calendar(calendar1, calendar2) | 두 캘린더의 작업 일정 교차점에 대한 계산을 수행하는 데 사용할 수 있는 [ICalendar](/tasks/python-net/aspose.tasks/icalendar/) 인스턴스를 가져옵니다. |
| make_standard_calendar(calendar) | 기본 표준 캘린더를 생성합니다. |
| make_24_hour_calendar(calendar) | 지정된 캘린더를 24시간 캘린더로 만듭니다.<br/>            24시간 캘린더는 주의 모든 요일이 24시간 연속 근무하는 캘린더입니다. |
| make_night_shift_calendar(calendar) | 지정된 캘린더를 야간 근무 캘린더로 만듭니다. |
| delete() | 프로젝트에서 캘린더를 제거합니다. |
| is_day_working(dt) | 캘린더에 따라 지정된 날짜가 근무일인지 여부를 판단합니다. |
| get_working_hours_time_span(start, finish) | 지정된 날짜 사이의 근무 시간량을 반환합니다. |
| get_task_finish_date_from_duration(task, duration) | 시작 날짜, 분할된 부분 및 작업 기간을 기준으로 작업의 완료 날짜와 시간을 계산합니다. |
| get_working_times(dt) | 지정된 날짜에 대한 작업 시간의 [WorkingTimeCollection](/tasks/python-net/aspose.tasks/workingtimecollection/)을 반환합니다. |
| get_previous_working_day_end(date) | 지정된 날짜를 기준으로 이전 근무 날짜의 종료 시점을 계산합니다. |
| get_next_working_day_start(date) | 지정된 날짜에 대한 다음 근무일 시작 시간을 계산합니다. |
| get_work_start(date) | 지정된 날짜와 시간부터 시작되는 다음 근무 시간 시작을 계산합니다. |
| is_empty() | 캘린더에 근무 시간이 정의되어 있지 않은지 여부를 반환합니다. |

### 또 보기

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

