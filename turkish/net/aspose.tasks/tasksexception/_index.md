---
title: "Sınıf TasksException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TasksException sınıfı. Standart iç istisna tipini temsil eder"
type: docs
weight: 2520
url: /tr/net/aspose.tasks/tasksexception/
---
## TasksException class

Standart iç istisna tipini temsil eder.

```csharp
public class TasksException : ApplicationException
```

## Örnekler

Bozuk bir projenin yapısını nasıl tespit edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// projenin yapısını kontrol et.
// Proje yapısı hatalıysa <see cref=\"TasksException\"> fırlatılacaktır.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


