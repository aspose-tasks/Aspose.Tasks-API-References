---
title: "Класс TaskCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TaskCollection. Представляет собой коллекцию объектов Task"
type: docs
weight: 2390
url: /ru/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Представляет коллекцию объектов [`Task`](../task/).

```csharp
public class TaskCollection : IList<Task>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Получает количество объектов, содержащихся в TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Возвращает элемент по указанному индексу. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Получает родительский проект объекта TaskCollection. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Добавляет новую задачу в коллекцию задач проекта на том же уровне структуры, что и последняя задача. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Вставляет новую задачу перед задачей с указанным идентификатором и на том же уровне структуры. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Добавляет новую задачу в коллекцию дочерних задач. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Добавьте указанную задачу в экземпляр класса `TaskCollection`. Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (это перенесёт расписание всех задач проекта (даты начала/окончания, устанавливает ранние/поздние даты) и вычислит зависимые поля, такие как запасы времени, трудозатраты и стоимость, идентификаторы и уровни структуры). Если ParentProject.CalculationMode установлен в Manual, метод автоматически вычислит только идентификатор задачи, уровень структуры и номера структуры. Если ParentProject.CalculationMode установлен в Automatic, метод автоматически перенесёт расписание всех задач проекта (даты начала/окончания, устанавливает ранние/поздние даты, вычисляет запасы времени, трудозатраты и стоимость, пересчитывает идентификаторы и уровни структуры). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Добавляет новую повторяющуюся задачу в коллекцию дочерних задач. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Проверяет, содержит ли коллекция указанный элемент. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Возвращает задачу с указанным Id, чей предок является родительской задачей этой коллекции. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Возвращает задачу с указанным Uid, чей предок является родительской задачей этой коллекции. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Это заглушка реализации метода Insert интерфейса IList, который только бросает NotSupportedException. |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Это заглушка реализации метода Remove интерфейса ICollection, который только бросает NotSupportedException. |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Преобразует объект TaskCollection в список объектов [`Task`](../task/). |

## Примеры

Показывает, как работать с коллекциями задач.

```csharp
var project = new Project();

// коллекция задач не является только для чтения и может быть расширена
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// создать задачи
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// вывести задачи проекта
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// задачу можно получить из коллекции по ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// или по UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// также можно добавить повторяющуюся задачу
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// возвращается первая задача в последовательности
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// коллекцию можно преобразовать в обычный список
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### См. также

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


