---
title: "Duration.Parse"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Duration. Mengonversi string yang ditentukan menjadi instance dari struct Duration"
type: docs
weight: 10
url: /id/net/aspose.tasks/duration/parse/
---
## Duration.Parse method

Mengonversi string yang ditentukan menjadi instance dari struct [`Duration`](../).

```csharp
public static Duration Parse(Project p, string value)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| p | Project | instance yang ditentukan dari kelas [`Project`](../../project/) untuk mengonversi durasi. |
| value | String | string yang ditentukan untuk dikonversi. |

### Nilai Kembali

Mengembalikan instance yang telah dikonversi dari struct [`Duration`](../).

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

* class [Project](../../project/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


