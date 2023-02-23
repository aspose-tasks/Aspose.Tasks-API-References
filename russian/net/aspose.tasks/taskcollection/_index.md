---
title: Class TaskCollection
second_title: Справочник по Aspose.Tasks для .NET API
description: Aspose.Tasks.TaskCollection сорт. Представляет наборTask объекты.
type: docs
weight: 2100
url: /ru/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Представляет набор[`Task`](../task/) объекты.

```csharp
public class TaskCollection : IList<Task>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Получает количество объектов, содержащихся в TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Получает значение, указывающее, доступна ли эта коллекция только для чтения. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Возвращает элемент по указанному индексу. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Получает родительский проект объекта TaskCollection. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Добавляет новую задачу в коллекцию задач проекта на том же уровне структуры, что и последняя задача. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Вставляет новую задачу перед задачей с указанным идентификатором и на том же уровне структуры. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Добавляет новую задачу в коллекцию дочерних задач. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Добавить указанную задачу в экземпляр`TaskCollection`class. Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (он перепланирует все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты) и вычисляет зависимые поля, такие как резервы, рабочие и поля затрат, идентификаторы и уровни структуры). Если ParentProject.CalculationMode имеет значение Manual, метод будет автоматически вычислять только идентификатор задачи, уровень структуры и номера структуры. даты, устанавливает ранние/поздние даты, вычисляет резервы, поля работы и затрат, пересчитывает идентификаторы и уровни структуры). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Добавляет новую повторяющуюся задачу в коллекцию дочерних задач. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Проверяет, содержит ли коллекция указанный элемент. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Возвращает задачу с указанным идентификатором, предком которой является родительская задача этой коллекции . |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Возвращает задачу с указанным Uid, чьим предком является родительская задача этой коллекции . |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Это заглушка метода Insert из IList, которая выдает только NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Это заглушка метода Remove из ICollection, которая выдает только NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Преобразует объект TaskCollection в список[`Task`](../task/) объекты. |

### Смотрите также

* class [Task](../task/)
* пространство имен [Aspose.Tasks](../../aspose.tasks/)
* сборка [Aspose.Tasks](../../)


