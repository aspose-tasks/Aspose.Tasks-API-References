---
title: "TaskCollection.Add"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskCollection. Добавляет указанную задачу к экземпляру класса TaskCollection. Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate после использования этого метода. Он перенастроит даты начала/завершения всех задач проекта, установит ранние/поздние даты и вычислит зависимые поля, такие как запасы времени, работа и стоимость, идентификаторы и уровни структуры. Если ParentProject.CalculationMode имеет значение Manual, метод автоматически вычислит только идентификатор задачи, уровень структуры и номера структуры. Если ParentProject.CalculationMode имеет значение Automatic, метод автоматически перенастраивает все задачи проекта, даты начала/завершения, устанавливает ранние/поздние даты, вычисляет запасы времени, работу и стоимость, пересчитывает идентификаторы и уровни структуры."
type: docs
weight: 50
url: /ru/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Добавьте указанную задачу к экземпляру класса [`TaskCollection`](../). Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (Он перенастроит все задачи проекта (даты начала/завершения, установит ранние/поздние даты) и вычислит зависимые поля, такие как запасы времени, работа и стоимость, идентификаторы и уровни структуры). Если ParentProject.CalculationMode имеет значение Manual, метод автоматически вычислит только идентификатор задачи, уровень структуры и номера структуры. Если ParentProject.CalculationMode имеет значение Automatic, метод автоматически перенастраивает все задачи проекта (даты начала/завершения, установит ранние/поздние даты, вычислит запасы времени, работу и стоимость, пересчитает идентификаторы и уровни структуры).

```csharp
public void Add(Task item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| элемент | Задача | указанная задача, которую следует добавить в эту коллекцию задач. |

## Примеры

Показывает, как переместить задачу под другого родителя.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// Получить задачи по идентификаторам
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// Добавление задачи 6 к другому родителю
task2.Children.Add(task);
```

### См. также

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

Добавляет новую задачу в коллекцию задач проекта на том же уровне структуры, что и последняя задача.

```csharp
public Task Add()
```

### Возвращаемое значение

возвращает только что добавленный экземпляр класса [`Task`](../../task/).

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Добавляет новую задачу в коллекцию дочерних задач.

```csharp
public Task Add(string taskName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| taskName | Строка | указанное имя задачи. |

### Возвращаемое значение

возвращает только что добавленный экземпляр класса [`Task`](../../task/).

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Добавляет новую повторяющуюся задачу в коллекцию дочерних задач.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| taskName | Строка | указанное имя задачи. |
| beforeTaskId | Int32 | Указанный идентификатор задачи, перед которой будет вставлена новая задача. |

### Возвращаемое значение

возвращает задачу, которая была вставлена перед задачей с указанным идентификатором.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException выбрасывается, если указанный идентификатор не является действительным идентификатором задачи. |

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Вставляет новую задачу перед задачей с указанным идентификатором и на том же уровне структуры.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Параметры, указанные для создания повторяющейся задачи. |

### Возвращаемое значение

возвращает только что добавленный экземпляр класса [`Task`](../../task/).

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Выбрасывается, если указанные параметры равны null. |
| ArgumentException | Выбрасывается, если указанные параметры недействительны. |

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

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


