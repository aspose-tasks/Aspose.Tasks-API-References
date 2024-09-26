---
title: Duration.Subtract
second_title: Aspose.Tasks for .NET API Reference
description: Duration method. Subtracts specified duration from this duration instance
type: docs
weight: 100
url: /net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

Subtracts specified duration from this duration instance.

```csharp
public Duration Subtract(Duration d)
```

| Parameter | Type | Description |
| --- | --- | --- |
| d | Duration | the specified [`Duration`](../) instance to subtract from this instance. |

### Return Value

New duration object that represents the value of this instance minus the specified duration value.

## Examples

Shows how to change a duration of tasks.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// get a task
var task1 = project.RootTask.Children.GetById(1);

// update the task duration
var duration1 = task1.Get(Tsk.Duration);

// subtract one day to the task 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// set a new duration to the task
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// get another task
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// change the duration by using actual time unit type
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// set a new duration to the task
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### See Also

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

Subtracts specified double value from this duration instance.

```csharp
public Duration Subtract(double val)
```

| Parameter | Type | Description |
| --- | --- | --- |
| val | Double | specified Double value to subtract from this instance. |

### Return Value

New duration object that represents the value of this instance minus the specified duration value.

## Examples

Shows how to change a duration of tasks.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// get a task
var task1 = project.RootTask.Children.GetById(1);

// update the task duration
var duration1 = task1.Get(Tsk.Duration);

// subtract one day to the task 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// set a new duration to the task
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// get another task
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// change the duration by using actual time unit type
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// set a new duration to the task
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### See Also

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


