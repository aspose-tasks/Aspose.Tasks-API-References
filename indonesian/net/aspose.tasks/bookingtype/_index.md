---
title: "Enum BookingType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.BookingType. Menentukan tipe pemesanan sumber daya"
type: docs
weight: 150
url: /id/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

Menentukan tipe pemesanan sumber daya.

```csharp
public enum BookingType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Menunjukkan nilai tidak didefinisikan dalam file proyek asli. |
| Committed | `0` | Menunjukkan tipe pemesanan yang dikomit. |
| Proposed | `1` | Menunjukkan tipe pemesanan yang diusulkan. |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

## Contoh

Menampilkan cara membaca/menulis properti Asn.BookingType.

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

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


