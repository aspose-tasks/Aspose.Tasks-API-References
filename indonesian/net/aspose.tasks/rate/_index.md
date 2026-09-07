---
title: "Kelas Rate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Rate. Mewakili definisi periode waktu dan tarif yang berlaku untuk sumber daya selama periode tersebut"
type: docs
weight: 1610
url: /id/net/aspose.tasks/rate/
---
## Rate class

Mewakili definisi periode waktu dan tarif yang berlaku untuk sumber daya selama periode tersebut.

```csharp
public class Rate
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | Mendapatkan atau mengatur biaya per penggunaan sumber daya. Nilai ini diambil dari tanggal saat ini jika tabel tarif ada untuk sumber daya. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | Mendapatkan atau mengatur tarif lembur per jam untuk sumber daya. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Mendapatkan atau mengatur satuan yang digunakan Microsoft Project untuk menampilkan tarif lembur. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | Mendapatkan atau mengatur tanggal ketika tarif mulai berlaku. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | Mendapatkan atau mengatur tanggal terakhir ketika tarif berlaku. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | Mendapatkan atau mengatur pengidentifikasi unik dari tabel tarif untuk sumber daya. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | Mendapatkan atau mengatur tarif standar per jam untuk sumber daya. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Mendapatkan atau mengatur satuan yang digunakan Microsoft Project untuk menampilkan tarif standar. |

## Contoh

Menampilkan cara bekerja dengan tarif sumber daya.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RateTable = RateType.A;
rate1.RatesFrom = new DateTime(2019, 1, 1, 8, 0, 0);
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;
rate1.OvertimeRate = 10m;
rate1.OvertimeRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;
rate2.CostPerUse = 2m;

// bekerja dengan proyek...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


