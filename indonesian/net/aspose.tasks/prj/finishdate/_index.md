---
title: "Prj.FinishDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Tanggal selesai dari sebuah proyek"
type: docs
weight: 330
url: /id/net/aspose.tasks/prj/finishdate/
---
## Prj.FinishDate field

Tanggal selesai proyek.

```csharp
public static readonly Key<DateTime, PrjKey> FinishDate;
```

## Contoh

Menampilkan cara menjadwal ulang proyek dari tanggal selesai alih-alih tanggal mulai.

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// Sekarang semua tanggal tugas (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) dihitung. Untuk mendapatkan jalur kritis kita perlu menghitung slack (dapat dipanggil di thread terpisah, tetapi hanya setelah perhitungan semua tanggal awal/akhir).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


