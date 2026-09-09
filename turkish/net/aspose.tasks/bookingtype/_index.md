---
title: "Enum BookingType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.BookingType enum. Bir kaynağın rezervasyon tipini belirtir."
type: docs
weight: 150
url: /tr/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

Bir kaynağın rezervasyon tipini belirtir.

```csharp
public enum BookingType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Değerin orijinal proje dosyasında tanımlanmadığını gösterir. |
| Committed | `0` | Committed rezervasyon tipini gösterir. |
| Proposed | `1` | Proposed rezervasyon tipini gösterir. |

## Açıklamalar

XML'e dışa aktarırken Tanımsız değerler sonuç XML'inden kaldırılacaktır.

## Örnekler

Asn.BookingType özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


