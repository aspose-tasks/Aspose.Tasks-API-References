---
title: Add
second_title: Справочник по Aspose.Tasks для .NET API
description: Добавить указанную задачу в экземпляр классаTaskCollectionaspose.tasks/taskcollection. Если ParentProject.CalculationMode имеет значение None пользователь должен вызвать Project.Recalculate после использования этого метода он перепланирует все задачи проекта даты начала/окончания устанавливает ранние/поздние даты и вычисляет зависимые поля такие как как резервы поля работы и затрат идентификаторы и уровни структуры. Если ParentProject.CalculationMode имеет значение Manual метод будет автоматически вычислять только идентификатор задачи уровень структуры и номера структуры. Если ParentProject.CalculationMode имеет значение Automatic метод автоматически перепланирует все задачи проекта даты начала/окончания устанавливает ранние/поздние даты вычисляет резервы поля работы и затрат пересчитывает идентификаторы и уровни контура.
type: docs
weight: 50
url: /ru/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Добавить указанную задачу в экземпляр класса[`TaskCollection`](../../taskcollection). Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (он перепланирует все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты) и вычисляет зависимые поля, такие как как резервы, поля работы и затрат, идентификаторы и уровни структуры). Если ParentProject.CalculationMode имеет значение Manual, метод будет автоматически вычислять только идентификатор задачи, уровень структуры и номера структуры. Если ParentProject.CalculationMode имеет значение Automatic, метод автоматически перепланирует все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты, вычисляет резервы, поля работы и затрат, пересчитывает идентификаторы и уровни контура).

```csharp
public void Add(Task item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| item | Task | указанная задача, которую необходимо добавить в эту коллекцию задач. |

### Смотрите также

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* пространство имен [Aspose.Tasks](../../taskcollection)
* сборка [Aspose.Tasks](../../../)

---

## Add() {#add}

Добавляет новую задачу в коллекцию задач проекта на том же уровне структуры последней задачи.

```csharp
public Task Add()
```

### Возвращаемое значение

возвращает только что добавленный экземпляр класса[`Task`](../../task).

### Смотрите также

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* пространство имен [Aspose.Tasks](../../taskcollection)
* сборка [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Добавляет новую задачу в коллекцию дочерних задач.

```csharp
public Task Add(string taskName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| taskName | String | указанное имя задачи. |

### Возвращаемое значение

возвращает только что добавленный экземпляр класса[`Task`](../../task).

### Смотрите также

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* пространство имен [Aspose.Tasks](../../taskcollection)
* сборка [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Добавляет новую повторяющуюся задачу в коллекцию дочерних задач.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| taskName | String | указанное имя задачи. |
| beforeTaskId | Int32 | Указанный идентификатор задачи, перед которой будет вставлена новая задача. |

### Возвращаемое значение

возвращает задачу, которая была вставлена перед задачей с указанным идентификатором.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException создается, если указанный идентификатор не является допустимым идентификатором задачи. |

### Смотрите также

* class [Task](../../task)
* class [TaskCollection](../../taskcollection)
* пространство имен [Aspose.Tasks](../../taskcollection)
* сборка [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Вставляет новую задачу перед задачей с указанным идентификатором и на том же уровне структуры.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Параметры указанные параметры для создания повторяющейся задачи. |

### Возвращаемое значение

возвращает только что добавленный экземпляр класса[`Task`](../../task).

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Вызывается, если указанные параметры равны нулю. |
| ArgumentException | Вызывается, если указанные параметры недействительны. |

### Смотрите также

* class [Task](../../task)
* class [RecurringTaskParameters](../../recurringtaskparameters)
* class [TaskCollection](../../taskcollection)
* пространство имен [Aspose.Tasks](../../taskcollection)
* сборка [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
