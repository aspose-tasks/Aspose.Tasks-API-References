---
title: "Aspose::Tasks::TaskCollection::Add метод"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks для C++"
description: "Добавляет новую задачу в коллекцию задач проекта на том же уровне структуры, что и последняя задача."
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

Добавляет новую задачу в коллекцию задач проекта на том же уровне структуры, что и последняя задача.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

Вставляет новую задачу перед задачей с указанным идентификатором и на том же уровне структуры.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| Параметр | Описание |
| --- | --- |
| параметры | Параметры, указанные для создания повторяющейся задачи. |

---

## Add (3 of 5) {#add_3}

Добавьте указанную задачу в экземпляр класса TaskCollection. Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (это перенесёт расписание всех задач проекта (даты начала/окончания, устанавливает ранние/поздние даты) и вычислит зависимые поля, такие как запасы времени, трудозатраты и стоимостные поля, идентификаторы и уровни структуры). Если ParentProject.CalculationMode имеет значение Manual, метод вычислит только идентификатор задачи, уровень структуры и номера структуры автоматически. Если ParentProject.CalculationMode имеет значение Automatic, метод автоматически перенесёт расписание всех задач проекта (даты начала/окончания, устанавливает ранние/поздние даты, вычисляет запасы времени, трудозатраты и стоимостные поля, пересчитывает идентификаторы и уровни структуры).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| Параметр | Описание |
| --- | --- |
| элемент | указанная задача, которую следует добавить в эту коллекцию задач. |

---

## Add (4 of 5) {#add_4}

Добавляет новую задачу в коллекцию дочерних задач.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| Параметр | Описание |
| --- | --- |
| taskName | указанное имя задачи. |

---

## Add (5 of 5) {#add_5}

Добавляет новую повторяющуюся задачу в коллекцию дочерних задач.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| Параметр | Описание |
| --- | --- |
| taskName | указанное имя задачи. |
| beforeTaskId | Указанный идентификатор задачи, перед которой будет вставлена новая задача. |

