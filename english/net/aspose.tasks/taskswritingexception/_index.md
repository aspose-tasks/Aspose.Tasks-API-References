---
title: Class TasksWritingException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TasksWritingException class. Represents the standard internal writing exception type
type: docs
weight: 2510
url: /net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

Represents the standard internal writing exception type.

```csharp
public class TasksWritingException : TasksLoggedException
```

## Properties

| Name | Description |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Gets the exception logging information. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Gets the exception operation information. |

## Examples

Shows how to read log text and type of exception to check problems with MPP export.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // export the project as an MPP file
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### See Also

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


