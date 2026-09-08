---
title: "Класс ValidationException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ValidationException. Представляет исключение, которое выбрасывается, когда при проверке сущности обнаруживаются ошибки."
type: docs
weight: 2790
url: /ru/net/aspose.tasks/validationexception/
---
## ValidationException class

Представляет исключение, которое выбрасывается, когда при проверке сущности обнаруживаются ошибки.

```csharp
public class ValidationException : ApplicationException
```

## Примеры

Показывает, как обрабатывать &lt;see cref="ValidationException"/&gt; при работе с повторяющимися задачами.

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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


