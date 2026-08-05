---
title: "Aspose::Tasks::WorkingTime::WorkingTime constructor"
linktitle: "WorkingTime"
articleTitle: "WorkingTime"
second_title: "Aspose.Tasks for C++"
description: "Initializes a new instance of the WorkingTime class with a interval with the specified start and finish times."
type: docs
weight: 10
url: /cpp/aspose.tasks/workingtime/workingtime/
---

## WorkingTime (1 of 3) {#workingtime_1}

Initializes a new instance of the WorkingTime class with a interval with the specified start and finish times.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::DateTime fromTime, System::DateTime toTime)
```

| Parameter | Description |
| --- | --- |
| fromTime | interval start time |
| toTime | interval end time |

---

## WorkingTime (2 of 3) {#workingtime_2}

Initializes a new instance of the WorkingTime class with an interval item with the specified start and finish times.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::TimeSpan fromTime, System::TimeSpan toTime)
```

| Parameter | Description |
| --- | --- |
| fromTime | Interval's start time represented by TimeSpan struct. |
| toTime | Interval's end time represented by TimeSpan struct. |

---

## WorkingTime (3 of 3) {#workingtime_3}

Initializes a new instance of the WorkingTime class with an interval item with the specified start and finish times.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(int32_t fromHours, int32_t toHours)
```

| Parameter | Description |
| --- | --- |
| fromHours | Interval's start time represented by whole number of hours (0-24). |
| toHours | Interval's end time represented by whole number of hours (0-24). |

