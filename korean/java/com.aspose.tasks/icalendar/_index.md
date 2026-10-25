---
title: "ICalendar"
second_title: "Aspose.Tasks for Java API Reference"
description: "날짜 및 기간의 다양한 계산에 사용할 수 있는 캘린더 추상화를 나타냅니다."
type: docs
weight: 376
url: /ko/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

날짜 및 기간의 다양한 계산에 사용할 수 있는 캘린더 추상화를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | 달력에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | 달력에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | 지정된 날짜에 대한 다음 작업일 시작 시간을 계산합니다. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | 지정된 날짜로부터 이전 작업일의 종료 시간을 계산합니다. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | 지정된 종료 날짜와 기간을 기준으로 시작 날짜를 반환합니다. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | 지정된 종료 날짜와 기간을 기준으로 시작 날짜를 반환합니다. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | 작업의 시작 날짜, 분할 부분 및 작업 기간을 기반으로 작업 종료 날짜와 시간을 계산합니다. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | 지정된 날짜와 시간부터 시작하는 다음 작업 시간 시작을 계산합니다. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | 지정된 날짜의 작업 시간 양을 반환합니다. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | WorkUnit을 반환합니다 - 지정된 날짜 시간 구간에 대한 작업 시간의 시작, 종료 및 기간. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | 지정된 날짜 사이의 작업 시간 양을 반환합니다. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | 지정된 날짜에 대한 작업 시간의 [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection)을 반환합니다. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | 달력에 따라 지정된 날짜가 작업일인지 여부를 판단합니다. |
| [isEmpty()](#isEmpty--) | 달력에 작업 시간이 정의되어 있지 않은지 여부를 반환합니다. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


달력에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 시작 날짜. |
| work | [Duration](../../com.aspose.tasks/duration) | 작업 기간. |

**Returns:**
java.util.Date - 종료 날짜.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


달력에 따라 지정된 작업 시간이 경과하는 날짜를 계산합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 시작 날짜. |
| 작업 | double | 작업 기간. |

**Returns:**
java.util.Date - 종료 날짜.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


지정된 날짜에 대한 다음 작업일 시작 시간을 계산합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 날짜 | java.util.Date | 다음 근무일 시작을 얻기 위한 날짜. |

**Returns:**
java.util.Date - 다음 근무일 시작 System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


지정된 날짜로부터 이전 작업일의 종료 시간을 계산합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 날짜 | java.util.Date | 이전 근무일 종료를 계산하기 위한 날짜. |

**Returns:**
java.util.Date - 이전 근무일 종료
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


지정된 종료 날짜와 기간을 기준으로 시작 날짜를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 완료 | java.util.Date | 지정된 완료 날짜. |
| duration | [Duration](../../com.aspose.tasks/duration) | 지정된 기간. |

**Returns:**
java.util.Date - 계산된 시작 날짜.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


지정된 종료 날짜와 기간을 기준으로 시작 날짜를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 완료 | java.util.Date | 지정된 완료 날짜. |
| 기간 | double | 지정된 기간. |

**Returns:**
java.util.Date - 계산된 시작 날짜.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


작업의 시작 날짜, 분할 부분 및 작업 기간을 기반으로 작업 종료 날짜와 시간을 계산합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 완료 날짜를 계산할 작업. |
|  | 기간 | double | 계산할 기간. |

작업이 요약이거나 null이거나 시작 날짜가 설정되지 않은 경우 DateTime.MinValue를 반환합니다. |

**Returns:**
java.util.Date - 주어진 시작 날짜와 기간에 대한 작업의 완료 날짜.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


지정된 날짜와 시간부터 시작하는 다음 작업 시간 시작을 계산합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 날짜 | java.util.Date | 날짜와 시간. |

**Returns:**
java.util.Date - 가장 가까운 근무 시간 시작.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


지정된 날짜의 작업 시간 양을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dt | java.util.Date | 근무 시간을 얻기 위한 날짜. |

**Returns:**
double - 지정된 날짜의 근무 시간.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


WorkUnit을 반환합니다 - 지정된 날짜 시간 구간에 대한 작업 시간의 시작, 종료 및 기간.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 구간의 시작 날짜. |
| 완료 | java.util.Date | 구간의 종료 날짜. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


지정된 날짜 사이의 작업 시간 양을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 구간의 시작 날짜. |
| 완료 | java.util.Date | 구간의 종료 날짜. |

**Returns:**
double - 캘린더 인스턴스에 따른 근무 시간 양.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


지정된 날짜에 대한 작업 시간의 [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection)을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dt | java.util.Date | 근무 시간을 얻기 위한 날짜. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


달력에 따라 지정된 날짜가 작업일인지 여부를 판단합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dt | java.util.Date | 해당 날짜가 근무일인지 확인하기 위한 날짜. |

**Returns:**
boolean - 해당 날짜가 근무일이면 true.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


달력에 작업 시간이 정의되어 있지 않은지 여부를 반환합니다.

**Returns:**
boolean - 캘린더에 근무 시간이 정의되지 않은 경우 True.
