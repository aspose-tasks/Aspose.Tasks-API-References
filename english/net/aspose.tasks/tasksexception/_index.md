---
title: Class TasksException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TasksException class. Represents the standard internal exception type
type: docs
weight: 2470
url: /net/aspose.tasks/tasksexception/
---
## TasksException class

Represents the standard internal exception type.

```csharp
public class TasksException : ApplicationException
```

## Examples

Shows how to detect broken project's structure.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// check the project's structure.
// The <see cref="TasksException"> will be thrown if the project structure is incorrect.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


