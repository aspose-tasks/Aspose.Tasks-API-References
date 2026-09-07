---
title: "Duration.ParseTimeSpan"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Duration. Mengurai string durasi dalam format PTHMS"
type: docs
weight: 130
url: /id/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

Menganalisis string durasi dalam format "PT--H--M--S--".

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | String | string yang ditentukan untuk diurai. |

### Nilai Kembali

mengembalikan instance yang diurai dari struct [`TimeSpan`](../timespan/).

## Contoh

Menampilkan cara mengonversi string menjadi rentang waktu.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### Lihat Juga

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


