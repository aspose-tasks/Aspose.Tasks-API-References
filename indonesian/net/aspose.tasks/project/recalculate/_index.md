---
title: "Project.Recalculate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Menjadwalkan ulang semua tugas proyek, ids, level outline, tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slacks, work, dan cost fields"
type: docs
weight: 1150
url: /id/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Menjadwalkan ulang semua ID tugas proyek, tingkat outline, tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, kerja, dan bidang biaya.

```csharp
public void Recalculate()
```

## Contoh

Menampilkan cara menjadwal ulang proyek dari tanggal mulai alih-alih tanggal selesai.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// Sekarang semua tanggal tugas (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) dihitung. Untuk mendapatkan jalur kritis kita perlu menghitung slack (dapat dipanggil di thread terpisah, tetapi hanya setelah perhitungan semua tanggal awal/akhir).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Menjadwalkan ulang semua ID tugas proyek, tingkat outline, tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, kerja, dan bidang biaya dengan validasi opsional.

```csharp
public void Recalculate(bool validate)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| validate | Boolean | Jika bernilai true, validasi perhitungan ulang akan dilakukan. Data apa yang divalidasi: Saat ini hanya validasi dasar rentang tanggal tugas dan tautan tugas yang diimplementasikan. Rentang tanggal tugas (mis. ActualStart - ActualFinish, EarlyStart - EarlyFinish, dll.) serta tanggal Tautan Tugas akan diperiksa terhadap kriteria tanggal bahwa tanggal mulai kurang atau sama dengan tanggal selesai. Jika salah satu kondisi di atas gagal, maka [`RecalculationValidationException`](../../recalculationvalidationexception/) akan dilempar. |

## Contoh

Menampilkan cara menghitung ulang proyek dengan validasi pasca.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // hitung ulang proyek dengan validasi pasca
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


