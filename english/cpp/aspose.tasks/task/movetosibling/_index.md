---
title: "Aspose::Tasks::Task::MoveToSibling method"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks for C++"
description: "Moves the current task at the same Outline Level before the specified task."
type: docs
weight: 1370
url: /cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

Moves the current task at the same Outline Level before the specified task. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| Parameter | Description |
| --- | --- |
| beforeTask | Task before which the current task will be inserted. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

Moves the current task at the same Outline Level before a task with the specified Id. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| Parameter | Description |
| --- | --- |
| beforeTaskId | Id ( Tsk::Id ) of a task before which the current task will be inserted. |

