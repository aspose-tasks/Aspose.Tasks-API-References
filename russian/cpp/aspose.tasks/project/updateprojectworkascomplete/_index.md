---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete метод"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks для C++"
description: "Обновляет всю работу как выполненную до указанной даты для всего проекта."
type: docs
weight: 2080
url: /ru/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

Обновляет всю работу как выполненную до указанной даты для всего проекта.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| Параметр | Описание |
| --- | --- |
| completeThrough | Дата, до которой обновляется работа как завершённая. |
| setZeroOrHundredPercentCompleteOnly | Если установлено в true, обновляет только те задачи как завершённые на 100%, у которых дата завершения раньше указанной даты complete-through. В противном случае вычисляет значение процента завершения на основе запланированных дат начала и даты complete-through. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

Обновляет всю работу как завершённую до указанной даты для заданного списка задач.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| Параметр | Описание |
| --- | --- |
| completeThrough | Дата, до которой обновляется работа как завершённая. |
| setZeroOrHundredPercentCompleteOnly | Если установлено в true, обновляет только те задачи как завершённые на 100%, у которых дата завершения раньше указанной даты complete-through. В противном случае вычисляет значение процента завершения на основе запланированных дат начала и даты complete-through. |
| taskCollection | List< Task > задач, для которых обновляется работа. |

