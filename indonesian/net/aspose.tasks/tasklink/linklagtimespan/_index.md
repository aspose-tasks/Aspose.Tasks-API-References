---
title: LinkLagTimeSpan
second_title: Aspose.Tasks untuk Referensi .NET API
description: Mendapat atau menyetel durasi lag bergantung pada LagFormat.
type: docs
weight: 50
url: /id/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Mendapat atau menyetel durasi lag, bergantung pada LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Saat mencoba menetapkan nilai untuk Tautan Tugas di mana LagFormat adalah TimeUnitType.Percent. |

### Perkataan

Lag link dapat berupa nilai persentase (LagFormat adalah TimeUnitType.Percent). Dalam hal ini durasi dihitung sebagai persentase durasi PredTask. Jika tidak, metode mengembalikan nilai TimeSpan yang mewakili lag Tautan Tugas.

### Lihat juga

* class [TaskLink](../)
* ruang nama [Aspose.Tasks](../../tasklink/)
* perakitan [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
