---
title: TaskCollection.Add
second_title: Aspose.Tasks for .NET API Reference
description: TaskCollection method. Add the specified task to the instance of the TaskCollection class. If ParentProject.CalculationMode is None user should invoke Project.Recalculate after using this method It will reschedule all project tasks start/finish dates sets early/late dates and calculate the dependent fields such as slacks work and cost fields ids and outline levels. If ParentProject.CalculationMode is Manual the method will calculate only task id outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all projects tasks automatically start/finish dates sets early/late dates calculates slacks work and cost fields recalculates ids and outline levels
type: docs
weight: 50
url: /net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Add the specified task to the instance of the [`TaskCollection`](../) class. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, ids and outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

```csharp
public void Add(Task item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | Task | the specified task which should be added to this task collection. |

## Examples

Shows how to move a task under another parent.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// Get Tasks by Ids
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// Adding Task 6 to another parent
task2.Children.Add(task);
```

### See Also

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

Adds new task to project tasks collection on the same outline level of the last task.

```csharp
public Task Add()
```

### Return Value

returns the newly added instance of the [`Task`](../../task/) class.

## Examples

Shows how to work with task collections.

```csharp
var project = new Project();

// the task collection is not read-only and can be extended
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// create tasks
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

// print project tasks
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

// a task can be taken from the collection by ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// or by UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// also one can add a recurring task
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

// the first task in a sequence is returned
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// the collection can be converted into a plain list
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### See Also

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Adds a new task to children tasks collection.

```csharp
public Task Add(string taskName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| taskName | String | the specified task name. |

### Return Value

returns the newly added instance of the [`Task`](../../task/) class.

## Examples

Shows how to work with task collections.

```csharp
var project = new Project();

// the task collection is not read-only and can be extended
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// create tasks
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

// print project tasks
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

// a task can be taken from the collection by ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// or by UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// also one can add a recurring task
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

// the first task in a sequence is returned
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// the collection can be converted into a plain list
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### See Also

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Adds a new recurring task to children tasks collection.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Parameter | Type | Description |
| --- | --- | --- |
| taskName | String | the specified task name. |
| beforeTaskId | Int32 | The specified id of a task before which a new task will be inserted. |

### Return Value

returns a task which was inserted before a task with the specified id.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException is thrown if the specified id is not a valid task id. |

## Examples

Shows how to work with task collections.

```csharp
var project = new Project();

// the task collection is not read-only and can be extended
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// create tasks
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

// print project tasks
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

// a task can be taken from the collection by ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// or by UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// also one can add a recurring task
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

// the first task in a sequence is returned
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// the collection can be converted into a plain list
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### See Also

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Inserts a new task before a task with the specified id and on the same outline level.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Parameter | Type | Description |
| --- | --- | --- |
| parameters | RecurringTaskParameters | The parameters the specified parameters for creation of recurring task. |

### Return Value

returns the newly added instance of the [`Task`](../../task/) class.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Thrown if the specified parameters are null. |
| ArgumentException | Thrown if the specified parameters are invalid. |

## Examples

Shows how to work with task collections.

```csharp
var project = new Project();

// the task collection is not read-only and can be extended
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// create tasks
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

// print project tasks
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

// a task can be taken from the collection by ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// or by UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// also one can add a recurring task
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

// the first task in a sequence is returned
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// the collection can be converted into a plain list
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### See Also

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


