---
title: "Aspose::Tasks::ICalendar::GetWorkingHours 메서드"
linktitle: "GetWorkingHours"
articleTitle: "GetWorkingHours"
second_title: "C++용 Aspose.Tasks"
description: "지정된 날짜의 작업 시간을 반환합니다."
type: docs
weight: 60
url: /ko/cpp/aspose.tasks/icalendar/getworkinghours/
---

## GetWorkingHours (1 of 2) {#getworkinghours_1}

지정된 날짜의 작업 시간을 반환합니다.

**Returns:** Working hours at the specified date.

```cpp
GetWorkingHours(System::DateTime dt)
```

| 매개변수 | 설명 |
| --- | --- |
| dt | 작업 시간을 가져올 날짜입니다. |

---

## GetWorkingHours (2 of 2) {#getworkinghours_2}

지정된 날짜/시간 간격에 대한 작업 시간의 시작, 종료 및 기간을 포함하는 WorkUnit을 반환합니다.

**Returns:** Instance of WorkUnit class containing Start, Finish and Duration of working hours.

```cpp
GetWorkingHours(System::DateTime start, System::DateTime finish)
```

| 매개변수 | 설명 |
| --- | --- |
| 시작 | 구간의 시작 날짜. |
| 끝 | 구간의 종료 날짜. |

