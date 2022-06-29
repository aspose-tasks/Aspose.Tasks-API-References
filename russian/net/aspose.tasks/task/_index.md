---
title: Task
second_title: Справочник по Aspose.Tasks для .NET API
description: Представляет задачу в проекте.
type: docs
weight: 2060
url: /ru/net/aspose.tasks/task/
---
## Task class

Представляет задачу в проекте.

```csharp
public class Task : IEquatable<Task>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Assignments](../../aspose.tasks/task/assignments) { get; } | Получает набор назначений ресурсов для этого объекта. |
| [Baselines](../../aspose.tasks/task/baselines) { get; set; } | Получает или задает набор базовых значений задачи. |
| [Children](../../aspose.tasks/task/children) { get; } | Получает коллекцию дочерних задач этого объекта. Объект TaskCollection, представляющий дочерние задачи. |
| [ExtendedAttributes](../../aspose.tasks/task/extendedattributes) { get; } | Получает объект ExtendedAttributeCollection, содержащий значения расширенного атрибута. |
| [OutlineCodes](../../aspose.tasks/task/outlinecodes) { get; set; } | Получает или устанавливает объект[`OutlineCodeCollection`](../outlinecodecollection). |
| [ParentProject](../../aspose.tasks/task/parentproject) { get; } | Получает родительский проект задачи. |
| [ParentTask](../../aspose.tasks/task/parenttask) { get; } | Получает родительскую задачу задачи. |
| [Predecessors](../../aspose.tasks/task/predecessors) { get; } | Получает объект[`TaskCollection`](../taskcollection), который содержит всех предшественников этого объекта Task. |
| [RecurringInfo](../../aspose.tasks/task/recurringinfo) { get; } | Получает экземпляр класса[`RecurringTaskInfo`](../recurringtaskinfo)для повторяющейся задачи; если задача не повторяющаяся, то возвращает null;  Информация об экземпляре[`RecurringTaskInfo`](../recurringtaskinfo)представлена только в формате файла mpp. |
| [SplitParts](../../aspose.tasks/task/splitparts) { get; } | Получает коллекцию SplitPart, представляющую части задачи. |
| [Successors](../../aspose.tasks/task/successors) { get; } | Получает объект[`TaskCollection`](../taskcollection), который содержит всех потомков этого объекта Task. |
| [TimephasedData](../../aspose.tasks/task/timephaseddata) { get; set; } | Получает или задает объект TimephasedDataCollection этой задачи. Поэтапный блок данных, связанный с задачей. |

## Методы

| Имя | Описание |
| --- | --- |
| [Clone](../../aspose.tasks/task/clone)() | Создает полную копию задачи без подзадач. |
| [Delete](../../aspose.tasks/task/delete)() | Удаляет задачу из коллекции задач родительского проекта и все ее назначения. |
| override [Equals](../../aspose.tasks/task/equals#equals_1)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [Equals](../../aspose.tasks/task/equals#equals)(Task) | Возвращает значение, указывающее, равен ли этот экземпляр заданной задаче. |
| [Get&lt;T&gt;](../../aspose.tasks/task/get)(Key&lt;T, TaskKey&gt;) | Возвращает значение, которому сопоставлено свойство в этом контейнере. |
| override [GetHashCode](../../aspose.tasks/task/gethashcode)() | Возвращает значение хэш-кода для этой задачи. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata)(DateTime, DateTime) | Возвращает[`TimephasedDataCollection`](../timephaseddatacollection)объект с[`TimephasedData`](./timephaseddata)значения в пределах заданных дат начала и окончания. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata_1)(DateTime, DateTime, TimephasedDataType) | Возвращает[`TimephasedDataCollection`](../timephaseddatacollection)объект с[`TimephasedData`](./timephaseddata)значения в пределах заданных дат начала и окончания указанного типа данных с временными интервалами. |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling_1)(int) | Перемещает текущую задачу на тот же уровень структуры перед задачей с указанным идентификатором. Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (он перепланирует все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты) и вычисляет зависимые поля, такие как как слаксы, поля работ и затрат, уровни структуры). Если ParentProject.CalculationMode имеет значение Manual, метод будет автоматически вычислять только идентификатор задачи, уровень структуры и номера структуры. Если ParentProject.CalculationMode имеет значение Automatic, метод автоматически перепланирует все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты, вычисляет резервы, поля работы и затрат, пересчитывает идентификаторы и уровни контура). |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling)(Task) | Перемещает текущую задачу на тот же уровень структуры перед указанной задачей. Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (он перепланирует все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты) и вычисляет зависимые поля, такие как как слаксы, поля работ и затрат, уровни структуры). Если ParentProject.CalculationMode имеет значение Manual, метод будет автоматически вычислять только идентификатор задачи, уровень структуры и номера структуры. Если ParentProject.CalculationMode имеет значение Automatic, метод автоматически перепланирует все задачи проекта (даты начала/окончания, устанавливает ранние/поздние даты, вычисляет резервы, поля работы и затрат, пересчитывает идентификаторы и уровни контура). |
| [OutlineIndent](../../aspose.tasks/task/outlineindent)() | Делает отступ задачи в структуре. |
| [OutlineOutdent](../../aspose.tasks/task/outlineoutdent)() | Продвигает задачу в структуре. |
| [SelectAllChildTasks](../../aspose.tasks/task/selectallchildtasks)() | Рекурсивно собирает все дочерние задачи этой задачи. |
| [Set&lt;T&gt;](../../aspose.tasks/task/set)(Key&lt;T, TaskKey&gt;, T) | Сопоставляет указанное свойство с указанным значением в этом контейнере. |
| override [ToString](../../aspose.tasks/task/tostring)() | Возвращает короткое строковое представление задачи. Точные детали представления не указаны и могут быть изменены. |

### Примечания

Задача есть представляющий один атомный патрон работы.

Можно использовать **Task** для планирования проекта путем создания задач и назначения им соответствующих ресурсов. Задачи в проекте организованы в виде корневой иерархической древовидной структуры с корневой задачей и поддеревьями дочерних задач.

Для построения дерева задач можно использовать специализированную коллекцию[`TaskCollection`](../taskcollection)обратившись к[`RootTask`](../project/roottask)свойство например:

```csharp
Project project = new Project();

// добавляем новые задачи
Task task1 = project.RootTask.Children.Add(); // добавляется родительская задача с пустым именем
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // вставляет задачу перед childTask3
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

// сохраняем проект в одном из доступных форматов
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

### Смотрите также

* пространство имен [Aspose.Tasks](../../aspose.tasks)
* сборка [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
