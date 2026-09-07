---
title: "Duration.IsEstimated"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Duration. Mengambil nilai yang menunjukkan apakah satuan waktu diperkirakan. Bendera yang menentukan apakah instance Duration ini diperkirakan"
type: docs
weight: 30
url: /id/net/aspose.tasks/duration/isestimated/
---
## Duration.IsEstimated property

Mendapatkan nilai yang menunjukkan apakah satuan waktu diperkirakan. Bendera yang menentukan apakah instance Duration ini diperkirakan.

```csharp
public bool IsEstimated { get; }
```

## Contoh

Menampilkan cara mengurai string dari string yang diformat khusus.

```csharp
var project = new Project();

// contoh durasi:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// di mana 1 - jumlah item (hari, minggu, dll), d - hari (h - jam, w - minggu) ? - bendera perkiraan, e - bendera berlalu

// coba mengurai durasi perkiraan
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// coba mengurai durasi perkiraan
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### Lihat Juga

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


