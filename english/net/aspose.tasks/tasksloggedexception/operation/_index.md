---
title: TasksLoggedException.Operation
second_title: Aspose.Tasks for .NET API Reference
description: TasksLoggedException property. Gets the exception operation information
type: docs
weight: 20
url: /net/aspose.tasks/tasksloggedexception/operation/
---
## TasksLoggedException.Operation property

Gets the exception operation information.

```csharp
public string Operation { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


