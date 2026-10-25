---
title: "CalendarException"
second_title: "Aspose.Tasks for Python via .NET API 참조"
description: 
type: docs
weight: 160
url: /ko/python-net/aspose.tasks/calendarexception/
---

## CalendarException class

캘린더의 예외적인 기간을 나타냅니다.

CalendarException 유형은 다음 멤버를 노출합니다:
## 생성자
| 이름 | 설명 |
| :- | :- |
| CalendarException() | 새로운 [CalendarException](/tasks/python-net/aspose.tasks/calendarexception/) 클래스 인스턴스를 초기화합니다. |
## 속성
| 이름 | 설명 |
| :- | :- |
| entered_by_occurrences | 반복 범위가 발생 횟수 입력으로 정의되는지 여부를 나타내는 값을 가져오거나 설정합니다.<br/>            False는 반복 범위가 종료 날짜 입력으로 정의됨을 지정합니다. |
| from_date | 예외 시간의 시작을 가져오거나 설정합니다. |
| to_date | 예외 시간의 끝을 가져오거나 설정합니다. |
| occurrences | 캘린더 예외가 유효한 발생 횟수를 가져오거나 설정합니다. |
| name | 예외의 이름을 가져오거나 설정합니다. |
| type | 예외 유형을 가져오거나 설정합니다. |
| period | 예외에 대한 반복 기간을 가져오거나 설정합니다. |
| days_of_week | 이 객체에 대한 DayTypeCollection을 가져옵니다.<br/>            예외가 유효한 요일들입니다. |
| month_item | 예외 반복이 예약된 월 항목을 가져오거나 설정합니다. |
| month_position | 월 내에서 월 항목의 위치를 가져오거나 설정합니다. |
| month | 예외 반복이 예약된 월을 가져오거나 설정합니다. |
| month_day | 예외 반복이 예약된 월의 일을 가져오거나 설정합니다. |
| day_working | 지정된 날짜 또는 요일 유형이 작업일인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| working_times | WorkingTimeCollection 객체를 가져오거나 설정합니다.<br/>            평일에 작업한 시간을 정의하는 작업 시간 컬렉션입니다. |
| parent_calendar | 이 객체의 상위 캘린더를 가져옵니다. |
## 메서드
| 이름 | 설명 |
| :- | :- |
| delete() | 부모 캘린더 CalendarExceptionCollection 객체에서 Exception 인스턴스를 삭제합니다. |
| check_exception(dt) | 지정된 datetime 구조체 인스턴스가 예외일인 경우 true를 반환합니다. |
| get_working_time() | 캘린더 예외에 대한 작업 시간을 반환합니다. |
| get_exception_dates() | 캘린더 예외가 적용되는 날짜를 반환합니다. |

### 또 보기

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

