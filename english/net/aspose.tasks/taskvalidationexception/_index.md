---
title: Class TaskValidationException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskValidationException class. Represents an exception which is thrown when errors are found in projects tasks after recalculation
type: docs
weight: 2480
url: /net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

Represents an exception which is thrown when errors are found in project's tasks after recalculation.

```csharp
public class TaskValidationException : RecalculationValidationException
```

## Properties

| Name | Description |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | Gets the task which caused the exception. |

## Examples

Shows on what conditions &lt;see cref="TaskValidationException" /&gt; exception can be thrown.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // accidentally set incorrect dates
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // run project recalculation with a flag to run validation   
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### See Also

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


