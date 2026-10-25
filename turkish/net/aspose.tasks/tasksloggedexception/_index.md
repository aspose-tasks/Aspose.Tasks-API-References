---
title: "Sınıf TasksLoggedException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TasksLoggedException sınıfı. Standart iç istisna tipini temsil eder"
type: docs
weight: 2530
url: /tr/net/aspose.tasks/tasksloggedexception/
---
## TasksLoggedException class

Standart iç istisna tipini temsil eder.

```csharp
public class TasksLoggedException : ApplicationException
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


