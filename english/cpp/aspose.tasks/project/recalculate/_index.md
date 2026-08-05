---
title: "Aspose::Tasks::Project::Recalculate method"
linktitle: "Recalculate"
articleTitle: "Recalculate"
second_title: "Aspose.Tasks for C++"
description: "Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields."
type: docs
weight: 1130
url: /cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| Parameter | Description |
| --- | --- |
| validate | If true the validation of recalculation will be performed. What data is validated: At the moment only basic validation of task and task link date ranges is implemented. Task 's date ranges (e.g. ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) as well as Task Links dates will be checked against the date criteria that start date is less or equal than finish date. If any of conditions described above is failed then RecalculationValidationException will be thrown. |

