---
title: "Aspose::Tasks::WorkingTime::WorkingTime конструктор"
linktitle: "WorkingTime"
articleTitle: "WorkingTime"
second_title: "Aspose.Tasks для C++"
description: "Инициализирует новый экземпляр класса WorkingTime с интервалом, заданным указанными временем начала и окончания."
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/workingtime/workingtime/
---

## WorkingTime (1 of 3) {#workingtime_1}

Инициализирует новый экземпляр класса WorkingTime с интервалом, заданным указанными временем начала и окончания.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::DateTime fromTime, System::DateTime toTime)
```

| Параметр | Описание |
| --- | --- |
| fromTime | время начала интервала |
| toTime | время окончания интервала |

---

## WorkingTime (2 of 3) {#workingtime_2}

Инициализирует новый экземпляр класса WorkingTime с элементом интервала, содержащим указанные время начала и окончания.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::TimeSpan fromTime, System::TimeSpan toTime)
```

| Параметр | Описание |
| --- | --- |
| fromTime | Время начала интервала представлено структурой TimeSpan. |
| toTime | Время окончания интервала представлено структурой TimeSpan. |

---

## WorkingTime (3 of 3) {#workingtime_3}

Инициализирует новый экземпляр класса WorkingTime с элементом интервала, содержащим указанные время начала и окончания.

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(int32_t fromHours, int32_t toHours)
```

| Параметр | Описание |
| --- | --- |
| fromHours | Время начала интервала представлено целым числом часов (0-24). |
| toHours | Время окончания интервала представлено целым числом часов (0-24). |

