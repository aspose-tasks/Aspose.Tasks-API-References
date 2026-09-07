---
title: "ResourceAssignment.SplitTask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceAssignment. Membagi tugas menjadi dua bagian"
type: docs
weight: 770
url: /id/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Membagi tugas menjadi dua bagian.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Awal gangguan kerja yang menjadi dasar pemisahan. |
| selesai | DateTime | Akhir gangguan kerja yang menjadi dasar pemisahan. |
| kalender | Calendar | Kalender yang menjadi dasar pemisahan. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Melemparkan pengecualian ketika tanggal mulai lebih kecil dari tanggal mulai penugasan. |
| ArgumentOutOfRangeException | Melemparkan pengecualian ketika tanggal selesai lebih besar dari tanggal selesai penugasan. |

## Contoh

Menampilkan cara menambahkan pemisahan untuk sebuah tugas.

```csharp
var project = new Project();

// Dapatkan kalender standar
var calendar = project.Get(Prj.Calendar);

// Atur pengaturan kalender proyek
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// Tambahkan tugas baru ke tugas root
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// Buat penugasan sumber daya baru dan hasilkan data berfase waktu
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// Bagi tugas menjadi 3 bagian.
// Berikan argumen tanggal mulai dan tanggal selesai ke metode SplitTask yang akan digunakan untuk pemisahan
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


