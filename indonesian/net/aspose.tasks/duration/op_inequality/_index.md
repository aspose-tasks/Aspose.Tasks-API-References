---
title: "Duration.op_Inequality"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Duration. Mengembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan"
type: docs
weight: 150
url: /id/net/aspose.tasks/duration/op_inequality/
---
## Duration Inequality operator

Kembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan.

```csharp
public static bool operator !=(Duration a, Duration b)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | Durasi | Durasi pertama. |
| b | Durasi | Durasi kedua. |

### Nilai Kembali

nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan

## Contoh

Menampilkan cara memeriksa kesetaraan durasi.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// kesetaraan durasi diperiksa terhadap timespan yang mendasarinya
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Lihat Juga

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


