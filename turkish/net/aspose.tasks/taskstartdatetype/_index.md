---
title: "Enum TaskStartDateType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskStartDateType enum. Bir görevin başlangıç tarihinin türünü belirtir"
type: docs
weight: 2450
url: /tr/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

Bir görevin başlangıç tarihinin türünü belirtir.

```csharp
public enum TaskStartDateType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Alan değerinin orijinal proje dosyasında tanımlı değildi. |
| ProjectStartDate | `0` | Proje başlangıç tarihi |
| CurrentDate | `1` | Geçerli tarih |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

## Örnekler

Görevin varsayılan başlangıç tarihinin 'CurrentDate' olarak nasıl ayarlanacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


