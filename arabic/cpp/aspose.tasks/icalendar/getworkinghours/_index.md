---
title: "Aspose::Tasks::ICalendar::GetWorkingHours طريقة"
linktitle: "GetWorkingHours"
articleTitle: "GetWorkingHours"
second_title: "Aspose.Tasks لـ C++"
description: "يعيد مقدار ساعات العمل في التاريخ المحدد."
type: docs
weight: 60
url: /ar/cpp/aspose.tasks/icalendar/getworkinghours/
---

## GetWorkingHours (1 of 2) {#getworkinghours_1}

يعيد مقدار ساعات العمل في التاريخ المحدد.

**Returns:** Working hours at the specified date.

```cpp
GetWorkingHours(System::DateTime dt)
```

| معامل | الوصف |
| --- | --- |
| dt | التاريخ للحصول على ساعات العمل. |

---

## GetWorkingHours (2 of 2) {#getworkinghours_2}

يرجع WorkUnit - البدء، الانتهاء والمدة لساعات العمل للفترة الزمنية المحددة.

**Returns:** Instance of WorkUnit class containing Start, Finish and Duration of working hours.

```cpp
GetWorkingHours(System::DateTime start, System::DateTime finish)
```

| معامل | الوصف |
| --- | --- |
| بدء | تاريخ البدء للفترة. |
| نهاية | تاريخ الانتهاء للفترة. |

