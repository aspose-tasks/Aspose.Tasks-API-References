---
title: "TaskLink.LinkLagTimeSpan"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TaskLink. Mendapatkan atau mengatur durasi keterlambatan tergantung pada LagFormat"
type: docs
weight: 50
url: /id/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Mendapatkan atau mengatur durasi lag, tergantung pada LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Saat mencoba mengatur nilai untuk TaskLinks di mana LagFormat adalah TimeUnitType.Percent. |

## Catatan

Keterlambatan tautan dapat berupa nilai persentase (LagFormat adalah TimeUnitType.Percent). Dalam kasus ini durasi dihitung sebagai persentase dari durasi PredTask. Jika tidak, metode mengembalikan nilai TimeSpan yang mewakili keterlambatan TaskLink.

### Lihat Juga

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


