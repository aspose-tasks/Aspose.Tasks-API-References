---
title: Task.Equals
second_title: Aspose.Tasks for .NET API Reference
description: Task method. Returns a value indicating whether this instance is equal to a specified task
type: docs
weight: 1330
url: /net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

Returns a value indicating whether this instance is equal to a specified task.

```csharp
public bool Equals(Task other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | Task | The specified task to compare with this instance. |

### Return Value

returns true if the specified task and this instance have equal unique ids.

## Examples

Shows how to iterate over task's assignments.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // display task's assignments
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### See Also

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The specified object to compare with this instance. |

### Return Value

returns true if the specified task and this instance have equal unique ids.

## Examples

Shows how to iterate over task's assignments.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // display task's assignments
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### See Also

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


