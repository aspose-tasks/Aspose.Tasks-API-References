---
title: "Sınıf ValidationException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ValidationException sınıfı. Bir varlığın doğrulaması sırasında hatalar bulunduğunda atılan bir istisnayı temsil eder."
type: docs
weight: 2790
url: /tr/net/aspose.tasks/validationexception/
---
## ValidationException class

Varlığın doğrulaması sırasında hatalar bulunduğunda fırlatılan bir istisnayı temsil eder.

```csharp
public class ValidationException : ApplicationException
```

## Örnekler

Tekrarlama görevleriyle çalışırken &lt;see cref=\"ValidationException\"/&gt; nasıl ele alınacağını gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


