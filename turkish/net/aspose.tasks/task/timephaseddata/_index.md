---
title: "Task.TimephasedData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Bu görevin bir TimephasedDataCollection nesnesini alır veya ayarlar. Bir görevle ilişkili zaman aşamalı veri bloğu"
type: docs
weight: 1220
url: /tr/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

Bu görevin TimephasedDataCollection nesnesini alır veya ayarlar. Görev ile ilişkili zaman aşamalı veri bloğu.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Açıklamalar

Okuma yalnızca XML biçimi için desteklenir.

## Örnekler

Görevin zaman aşamalı verileri üzerinde nasıl yineleme yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Ayrıca Bakınız

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


