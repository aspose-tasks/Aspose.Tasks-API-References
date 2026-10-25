---
title: "TasksLoggedException.LogText"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TasksLoggedException özelliği. İstisna günlükleme bilgilerini alır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/tasksloggedexception/logtext/
---
## TasksLoggedException.LogText property

İstisna günlükleme bilgilerini alır.

```csharp
public string LogText { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


