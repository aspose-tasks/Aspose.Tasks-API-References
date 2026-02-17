---
title: Class TasksReadingException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TasksReadingException class. Represents the standard internal reading exception type
type: docs
weight: 2520
url: /net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

Represents the standard internal reading exception type.

```csharp
public class TasksReadingException : TasksLoggedException
```

## Properties

| Name | Description |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Gets the exception logging information. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Gets the exception operation information. |

## Examples

Shows how to handle project' reading/writing exceptions.

```csharp
try
{
    var project = new Project(DataDir + "project.mpp");
    project.Save(OutDir + "HandleExceptions_out.mpp", SaveFileFormat.Mpp);
}
catch (TasksReadingException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    Console.WriteLine("Log: ");
    Console.WriteLine(ex.LogText);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### See Also

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


