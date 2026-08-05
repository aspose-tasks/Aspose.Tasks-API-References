---
title: "Aspose::Tasks::TaskCollection::Add method"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks for C++"
description: "Adds new task to project tasks collection on the same outline level of the last task."
type: docs
weight: 10
url: /cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

Adds new task to project tasks collection on the same outline level of the last task.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

Inserts a new task before a task with the specified id and on the same outline level.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| Parameter | Description |
| --- | --- |
| parameters | The parameters the specified parameters for creation of recurring task. |

---

## Add (3 of 5) {#add_3}

Add the specified task to the instance of the TaskCollection class. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, ids and outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| Parameter | Description |
| --- | --- |
| item | the specified task which should be added to this task collection. |

---

## Add (4 of 5) {#add_4}

Adds a new task to children tasks collection.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| Parameter | Description |
| --- | --- |
| taskName | the specified task name. |

---

## Add (5 of 5) {#add_5}

Adds a new recurring task to children tasks collection.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| Parameter | Description |
| --- | --- |
| taskName | the specified task name. |
| beforeTaskId | The specified id of a task before which a new task will be inserted. |

