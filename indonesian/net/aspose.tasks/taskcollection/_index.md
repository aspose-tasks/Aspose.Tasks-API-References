---
title: "Kelas TaskCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TaskCollection. Mewakili kumpulan objek Task"
type: docs
weight: 2390
url: /id/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Mewakili kumpulan objek [`Task`](../task/).

```csharp
public class TaskCollection : IList<Task>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Mendapatkan jumlah objek yang terdapat dalam TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Mengembalikan elemen pada indeks yang ditentukan. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Mendapatkan proyek induk dari objek TaskCollection. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Menambahkan tugas baru ke koleksi tugas proyek pada tingkat outline yang sama dengan tugas terakhir. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Menyisipkan tugas baru sebelum tugas dengan id yang ditentukan dan pada tingkat outline yang sama. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Menambahkan tugas baru ke koleksi tugas anak. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Tambahkan tugas yang ditentukan ke instance kelas `TaskCollection`. Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwalkan ulang semua tugas proyek (tanggal mulai/selesai, mengatur tanggal awal/akhir) dan menghitung bidang yang bergantung seperti slack, bidang kerja dan biaya, id, serta tingkat outline). Jika ParentProject.CalculationMode adalah Manual, metode ini hanya akan menghitung id tugas, tingkat outline, dan nomor outline secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwalkan ulang semua tugas proyek secara otomatis (tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya, menghitung ulang id dan tingkat outline). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Menambahkan tugas berulang baru ke koleksi tugas anak. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Memeriksa apakah koleksi berisi item yang ditentukan. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Mengembalikan tugas dengan Id yang ditentukan yang nenek moyangnya adalah tugas induk dari koleksi ini. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Mengembalikan tugas dengan Uid yang ditentukan yang nenek moyangnya adalah tugas induk dari koleksi ini. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Ini adalah implementasi stub dari metode Insert milik IList, yang hanya melempar NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Ini adalah implementasi stub dari metode Remove milik ICollection, yang hanya melempar NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Mengonversi objek TaskCollection menjadi daftar objek [`Task`](../task/). |

## Contoh

Menampilkan cara bekerja dengan koleksi tugas.

```csharp
var project = new Project();

// koleksi tugas tidak bersifat read-only dan dapat diperluas
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// buat tugas
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// cetak tugas proyek
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// tugas dapat diambil dari koleksi dengan ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// atau dengan UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// juga dapat menambahkan tugas berulang
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// tugas pertama dalam urutan dikembalikan
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// koleksi dapat dikonversi menjadi daftar biasa
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Lihat Juga

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


