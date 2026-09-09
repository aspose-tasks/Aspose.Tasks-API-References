---
title: "TasksLoggedException.Operation"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TasksLoggedException özelliği. İstisna işlem bilgilerini alır."
type: docs
weight: 20
url: /tr/net/aspose.tasks/tasksloggedexception/operation/
---
## TasksLoggedException.Operation property

İstisna işlem bilgilerini alır.

```csharp
public string Operation { get; }
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


