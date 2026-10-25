---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment yöntemi. Belirtilen tarih saat aralığı için zaman aşamalı iş miktarını alır"
type: docs
weight: 730
url: /tr/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

Belirtilen tarih zaman aralığı için zaman aşamalı iş miktarını alır.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Tarih saat aralığının başlangıcı. |
| bitiş | DateTime | Tarih saat aralığının sonu. |
| timephasedDataType | TimephasedDataType | Kullanılacak zaman aşamalı verinin türü. |

## Örnekler

Keyfi bir tarih saat aralığı için atamanın işini nasıl hesaplayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// Her saat için atamanın işini yazdır.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### Ayrıca Bakınız

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

Belirtilen tarih zaman aralığı için zaman aşamalı iş miktarını alır.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Tarih saat aralığının başlangıcı. |
| bitiş | DateTime | Tarih saat aralığının sonu. |

### Ayrıca Bakınız

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


