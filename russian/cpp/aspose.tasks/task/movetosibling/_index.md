---
title: "Aspose::Tasks::Task::MoveToSibling метод"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks для C++"
description: "Перемещает текущую задачу на том же уровне структуры перед указанной задачей."
type: docs
weight: 1370
url: /ru/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

Перемещает текущую задачу на том же уровне Outline перед указанной задачей. Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (это перенесёт все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты) и вычислит зависимые поля, такие как запасы времени, трудозатраты и стоимость, уровни Outline). Если ParentProject.CalculationMode имеет значение Manual, метод автоматически вычислит только идентификатор задачи, уровень Outline и номера Outline. Если ParentProject.CalculationMode имеет значение Automatic, метод автоматически перенесёт все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты, вычисляет запасы времени, трудозатраты и стоимость, пересчитывает идентификаторы и уровни Outline).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| Параметр | Описание |
| --- | --- |
| beforeTask | Задача, перед которой будет вставлена текущая задача. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

Перемещает текущую задачу на том же уровне структуры перед задачей с указанным Id. Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (это перенесёт график всех задач проекта (даты начала/окончания, устанавливает ранние/поздние даты) и вычислит зависимые поля, такие как запасы времени, трудозатраты и стоимость, уровни структуры). Если ParentProject.CalculationMode имеет значение Manual, метод автоматически вычислит только Id задачи, уровень структуры и номера структуры. Если ParentProject.CalculationMode имеет значение Automatic, метод автоматически перенесёт график всех задач проекта (даты начала/окончания, устанавливает ранние/поздние даты, вычисляет запасы времени, трудозатраты и стоимость, пересчитывает Id и уровни структуры).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| Параметр | Описание |
| --- | --- |
| beforeTaskId | Id ( Tsk::Id ) задачи, перед которой будет вставлена текущая задача. |

