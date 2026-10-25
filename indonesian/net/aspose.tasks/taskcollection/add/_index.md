---
title: "TaskCollection.Add"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskCollection. Menambahkan tugas yang ditentukan ke instance kelas TaskCollection. Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate setelah menggunakan metode ini. Itu akan menjadwalkan ulang semua tanggal mulai/selesai tugas proyek, mengatur tanggal awal/akhir, dan menghitung bidang-bidang yang bergantung seperti slack, kerja, dan biaya, serta ID dan level outline. Jika ParentProject.CalculationMode adalah Manual, metode ini hanya akan menghitung ID tugas, level outline, dan nomor outline secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwalkan ulang semua tugas proyek secara otomatis, mengatur tanggal mulai/selesai, tanggal awal/akhir, menghitung slack, kerja, dan biaya, serta menghitung ulang ID dan level outline."
type: docs
weight: 50
url: /id/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Tambahkan tugas yang ditentukan ke instance kelas [`TaskCollection`](../). Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwalkan ulang semua tugas proyek (tanggal mulai/selesai, mengatur tanggal awal/akhir) dan menghitung bidang-bidang yang bergantung seperti slack, kerja, dan biaya, serta ID dan level outline). Jika ParentProject.CalculationMode adalah Manual, metode ini akan menghitung hanya ID tugas, level outline, dan nomor outline secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwalkan ulang semua tugas proyek secara otomatis (tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, kerja, dan biaya, menghitung ulang ID dan level outline).

```csharp
public void Add(Task item)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | Tugas | tugas yang ditentukan yang harus ditambahkan ke koleksi tugas ini. |

## Contoh

Menampilkan cara memindahkan tugas ke bawah induk lain.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// Dapatkan Tugas berdasarkan Id
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// Menambahkan Tugas 6 ke induk lain
task2.Children.Add(task);
```

### Lihat Juga

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

Menambahkan tugas baru ke koleksi tugas proyek pada tingkat outline yang sama dengan tugas terakhir.

```csharp
public Task Add()
```

### Nilai Kembali

mengembalikan instance baru yang ditambahkan dari kelas [`Task`](../../task/).

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Menambahkan tugas baru ke koleksi tugas anak.

```csharp
public Task Add(string taskName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| taskName | String | nama tugas yang ditentukan. |

### Nilai Kembali

mengembalikan instance baru yang ditambahkan dari kelas [`Task`](../../task/).

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Menambahkan tugas berulang baru ke koleksi tugas anak.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| taskName | String | nama tugas yang ditentukan. |
| beforeTaskId | Int32 | Id yang ditentukan dari sebuah tugas sebelum mana tugas baru akan disisipkan. |

### Nilai Kembali

mengembalikan tugas yang disisipkan sebelum tugas dengan id yang ditentukan.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException dilemparkan jika id yang ditentukan bukan id tugas yang valid. |

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Menyisipkan tugas baru sebelum tugas dengan id yang ditentukan dan pada tingkat outline yang sama.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Parameter yang ditentukan untuk pembuatan tugas berulang. |

### Nilai Kembali

mengembalikan instance baru yang ditambahkan dari kelas [`Task`](../../task/).

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | Dilemparkan jika parameter yang ditentukan bernilai null. |
| ArgumentException | Dilemparkan jika parameter yang ditentukan tidak valid. |

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

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


