---
title: TaskLinkCollection.Add
second_title: Aspose.Tasks for .NET API Reference
description: TaskLinkCollection method. Returns an instance of FinishStart TaskLink which has been added to the TaskLinkCollection object
type: docs
weight: 40
url: /net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Returns an instance of Finish-Start [`TaskLink`](../../tasklink/) which has been added to the TaskLinkCollection object.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pred | Task | Predecessor task. |
| succ | Task | Successor task. |

### Return Value

a task link instance which has been added to this object.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | If any of input tasks is equal to null then ArgumentNullException will be thrown. |

## Examples

Shows how to work with task link collections.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// get tasks
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// link the tasks
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// print links among the tasks
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// edit link by index access
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// remove all task links
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### See Also

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

Returns an instance of [`TaskLink`](../../tasklink/) which has been added to the TaskLinkCollection object.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pred | Task | Predecessor task. |
| succ | Task | Successor task. |
| linkType | TaskLinkType | Link type [`TaskLinkType`](../../tasklinktype/) |

### Return Value

a task link instance which has been added to this object.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | If any of input tasks is equal to null then ArgumentNullException will be thrown. |

## Examples

Shows how to work with task link collections.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// get tasks
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// link the tasks
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// print links among the tasks
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// edit link by index access
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// remove all task links
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### See Also

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

Returns an instance of [`TaskLink`](../../tasklink/) which has been added to the TaskLinkCollection object.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pred | Task | Predecessor task. |
| succ | Task | Successor task. |
| linkType | TaskLinkType | Link type [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Link lag [`Duration`](../../duration/). |

### Return Value

a task link which has been added to this object.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | If any of input tasks is equal to null then ArgumentNullException will be thrown. |

## Examples

Shows how to work with task link collections.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// get tasks
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// link the tasks
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// print links among the tasks
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// edit link by index access
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// remove all task links
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### See Also

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

This is the stub implementation of ICollection's Add method, that only throws NotSupportedException

```csharp
public void Add(TaskLink item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | TaskLink | The item to add. |

### See Also

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


