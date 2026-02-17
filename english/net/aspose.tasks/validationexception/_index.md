---
title: Class ValidationException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ValidationException class. Represents an exception which is thrown when errors are found during validation of entity
type: docs
weight: 2770
url: /net/aspose.tasks/validationexception/
---
## ValidationException class

Represents an exception which is thrown when errors are found during validation of entity.

```csharp
public class ValidationException : ApplicationException
```

## Examples

Shows how to handle &lt;see cref="ValidationException"/&gt; while working with recurrence tasks.

```csharp
try
{
    var project = new Project();
    var parameters = new RecurringTaskParameters { TaskName = "t1", Duration = project.GetDuration(1, TimeUnitType.Day), RecurrencePattern = null };
    project.RootTask.Children.Add(parameters);
}
catch (ValidationException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


