---
title: "Aspose::Tasks::WorkingTime::WorkingTime 생성자"
linktitle: "WorkingTime"
articleTitle: "WorkingTime"
second_title: "C++용 Aspose.Tasks"
description: "지정된 시작 및 종료 시간으로 구간을 갖는 WorkingTime 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/workingtime/workingtime/
---

## WorkingTime (1 of 3) {#workingtime_1}

지정된 시작 및 종료 시간으로 구간을 갖는 WorkingTime 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::DateTime fromTime, System::DateTime toTime)
```

| 매개변수 | 설명 |
| --- | --- |
| fromTime | 구간 시작 시간 |
| toTime | 구간 종료 시간 |

---

## WorkingTime (2 of 3) {#workingtime_2}

지정된 시작 및 종료 시간을 가진 구간 항목으로 WorkingTime 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::TimeSpan fromTime, System::TimeSpan toTime)
```

| 매개변수 | 설명 |
| --- | --- |
| fromTime | 구간의 시작 시간은 TimeSpan 구조체로 표시됩니다. |
| toTime | 구간의 종료 시간은 TimeSpan 구조체로 표시됩니다. |

---

## WorkingTime (3 of 3) {#workingtime_3}

지정된 시작 및 종료 시간을 가진 구간 항목으로 WorkingTime 클래스의 새 인스턴스를 초기화합니다.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(int32_t fromHours, int32_t toHours)
```

| 매개변수 | 설명 |
| --- | --- |
| fromHours | 구간의 시작 시간은 0-24 범위의 정수 시간으로 표시됩니다. |
| toHours | 구간의 종료 시간은 0-24 범위의 정수 시간으로 표시됩니다. |

