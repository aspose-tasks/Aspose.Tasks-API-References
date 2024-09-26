---
title: Duration.Add
second_title: Aspose.Tasks for .NET API Reference
description: Duration method. Adds specified duration to this duration
type: docs
weight: 60
url: /net/aspose.tasks/duration/add/
---
## Add(Duration) {#add}

Adds specified duration to this duration.

```csharp
public Duration Add(Duration d)
```

| Parameter | Type | Description |
| --- | --- | --- |
| d | Duration | specified [`Duration`](../) to add to this instance. |

### Return Value

New duration object that represents the value of this instance plus the specified duration value.

## Examples

Shows how to update a duration of tasks.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// get a task
var task1 = project.RootTask.Children.GetById(1);

// update the task duration
var duration1 = task1.Get(Tsk.Duration);

// add one day to the task 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// set a new duration to the task
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// get another task
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// change the duration by using actual time unit type
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// set a new duration to the task
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### See Also

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Add(double) {#add_1}

Adds specified double value to this duration.

```csharp
public Duration Add(double val)
```

| Parameter | Type | Description |
| --- | --- | --- |
| val | Double | the specified Double value to add to this instance. |

### Return Value

New duration object that represents the value of this instance plus the specified duration value.

## Examples

Shows how to update a duration of tasks.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// get a task
var task1 = project.RootTask.Children.GetById(1);

// update the task duration
var duration1 = task1.Get(Tsk.Duration);

// add one day to the task 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// set a new duration to the task
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// get another task
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// change the duration by using actual time unit type
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// set a new duration to the task
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### See Also

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


