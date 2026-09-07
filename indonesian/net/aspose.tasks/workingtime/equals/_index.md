---
title: "WorkingTime.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode WorkingTime. Memeriksa bahwa objek-objek tersebut sama"
type: docs
weight: 40
url: /id/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

Memeriksa bahwa objek-objek tersebut sama.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | Objek kedua untuk dibandingkan. |

### Nilai Kembali

True jika objek-objek tersebut sama, false jika tidak.

## Contoh

Menampilkan cara memeriksa kesetaraan waktu kerja.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// Kesetaraan kalender diperiksa terhadap tanggal from dan to dari waktu kerja.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Lihat Juga

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


