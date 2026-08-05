---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete method"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks for C++"
description: "Updates all work as complete through a specified date for the entire project."
type: docs
weight: 2080
url: /cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

Updates all work as complete through a specified date for the entire project.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| Parameter | Description |
| --- | --- |
| completeThrough | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

Updates all work as complete through a specified date for the specified list of tasks.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| Parameter | Description |
| --- | --- |
| completeThrough | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |
| taskCollection | List< Task > of tasks to update work for. |

