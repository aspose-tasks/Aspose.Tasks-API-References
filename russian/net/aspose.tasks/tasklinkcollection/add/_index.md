---
title: TaskLinkCollection.Add
second_title: Справочник по Aspose.Tasks для .NET API
description: TaskLinkCollection метод. Возвращает экземпляр FinishStartTaskLink который был добавлен в объект TaskLinkCollection.
type: docs
weight: 40
url: /ru/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Возвращает экземпляр Finish-Start[`TaskLink`](../../tasklink/) который был добавлен в объект TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pred | Task | Задача предшественника. |
| succ | Task | Задача преемника. |

### Возвращаемое значение

экземпляр ссылки на задачу, который был добавлен к этому объекту.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Если какая-либо из входных задач равна нулю, тоArgumentNullException будет брошен. |

### Смотрите также

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* пространство имен [Aspose.Tasks](../../tasklinkcollection/)
* сборка [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

Возвращает экземпляр[`TaskLink`](../../tasklink/) который был добавлен в объект TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pred | Task | Задача предшественника. |
| succ | Task | Задача преемника. |
| linkType | TaskLinkType | Тип ссылки[`TaskLinkType`](../../tasklinktype/) |

### Возвращаемое значение

экземпляр ссылки на задачу, который был добавлен к этому объекту.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Если какая-либо из входных задач равна нулю, тоArgumentNullException будет брошен. |

### Смотрите также

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* пространство имен [Aspose.Tasks](../../tasklinkcollection/)
* сборка [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

Возвращает экземпляр[`TaskLink`](../../tasklink/) который был добавлен в объект TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pred | Task | Задача предшественника. |
| succ | Task | Задача преемника. |
| linkType | TaskLinkType | Тип ссылки[`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Задержка связи[`Duration`](../../duration/). |

### Возвращаемое значение

ссылка на задачу, которая была добавлена к этому объекту.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Если какая-либо из входных задач равна нулю, тоArgumentNullException будет брошен. |

### Смотрите также

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* пространство имен [Aspose.Tasks](../../tasklinkcollection/)
* сборка [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Это заглушка реализации метода Add ICollection, которая выдает только NotSupportedException

```csharp
public void Add(TaskLink item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| item | TaskLink | Элемент для добавления. |

### Смотрите также

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* пространство имен [Aspose.Tasks](../../tasklinkcollection/)
* сборка [Aspose.Tasks](../../../)


