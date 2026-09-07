---
title: "Enum RateFormatType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.RateFormatType enum. Menentukan satuan yang digunakan Microsoft Project untuk menampilkan tarif"
type: docs
weight: 1640
url: /id/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

Menentukan satuan yang digunakan oleh Microsoft Project untuk menampilkan tarif.

```csharp
public enum RateFormatType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Nilai tidak didefinisikan dalam file proyek asli. |
| Minute | `0` | Menit (\"min\") |
| Hour | `1` | Jam (\"hr\") |
| Day | `2` | Hari (\"day\") |
| Week | `3` | Minggu (\"wk\") |
| Month | `4` | Bulan (\"mo\") |
| Year | `5` | Tahun (\"yr\") |
| MaterialResourceRate | `6` | Tarif sumber daya material (kosong) |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

## Contoh

Menampilkan cara membaca/menulis properti Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


