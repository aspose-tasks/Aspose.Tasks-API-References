---
title: "Sınıf TasksReadingException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TasksReadingException sınıfı. Standart iç okuma istisna tipini temsil eder"
type: docs
weight: 2540
url: /tr/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

Standart iç okuma istisna tipini temsil eder.

```csharp
public class TasksReadingException : TasksLoggedException
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | İstisna günlükleme bilgilerini alır. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | İstisna işlem bilgilerini alır. |

## Örnekler

Projenin okuma/yazma istisnalarını nasıl ele alacağınızı gösterir.

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

### Ayrıca Bakınız

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


