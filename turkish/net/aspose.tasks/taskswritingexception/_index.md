---
title: "Sınıf TasksWritingException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TasksWritingException sınıfı. Standart iç yazma istisna tipini temsil eder"
type: docs
weight: 2560
url: /tr/net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

Standart iç yazma istisna tipini temsil eder.

```csharp
public class TasksWritingException : TasksLoggedException
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | İstisna günlükleme bilgilerini alır. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | İstisna işlem bilgilerini alır. |

## Örnekler

MPP dışa aktarma ile ilgili sorunları kontrol etmek için günlük metnini ve istisna türünü nasıl okuyacağınızı gösterir.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // projeyi bir MPP dosyası olarak dışa aktar
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### Ayrıca Bakınız

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


