---
title: "Aspose::Tasks::Calendar::GetWorkingHours метод"
linktitle: "GetWorkingHours"
articleTitle: "GetWorkingHours"
second_title: "Aspose.Tasks для C++"
description: "Возвращает количество рабочих часов на указанную дату."
type: docs
weight: 190
url: /ru/cpp/aspose.tasks/calendar/getworkinghours/
---

## GetWorkingHours (1 of 2) {#getworkinghours_1}

Возвращает количество рабочих часов на указанную дату.

**Returns:** Working hours at the specified date.

```cpp
GetWorkingHours(System::DateTime dt)
```

| Параметр | Описание |
| --- | --- |
| dt | Дата, для которой необходимо получить рабочие часы. |

---

## GetWorkingHours (2 of 2) {#getworkinghours_2}

Возвращает WorkUnit - Start, Finish и Duration рабочих часов для указанного интервала даты и времени.

**Returns:** Instance of WorkUnit class containing Start, Finish and Duration of working hours.

```cpp
GetWorkingHours(System::DateTime start, System::DateTime finish)
```

| Параметр | Описание |
| --- | --- |
| начало | Дата начала интервала. |
| конец | Дата окончания интервала. |

