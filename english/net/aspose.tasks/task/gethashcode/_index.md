---
title: Task.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: Task method. Returns a hash code value for this Task
type: docs
weight: 1350
url: /net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

Returns a hash code value for this Task.

```csharp
public override int GetHashCode()
```

### Return Value

returns a hash code value for this object.

## Examples

Shows how to get a hash code of a task.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// the hash code of a task is based on task's uid and name
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### See Also

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


