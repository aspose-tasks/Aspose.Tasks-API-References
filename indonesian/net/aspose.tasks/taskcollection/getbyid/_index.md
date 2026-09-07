---
title: "TaskCollection.GetById"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskCollection. Mengembalikan tugas dengan Id yang ditentukan yang induknya adalah tugas induk dari koleksi ini."
type: docs
weight: 70
url: /id/net/aspose.tasks/taskcollection/getbyid/
---
## TaskCollection.GetById method

Mengembalikan tugas dengan Id yang ditentukan yang nenek moyangnya adalah tugas induk dari koleksi ini.

```csharp
public Task GetById(int id)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| id | Int32 | TaskEntity Id |

### Nilai Kembali

mengembalikan instance dari kelas [`Task`](../../task/) dengan id yang ditentukan, yang merupakan tugas induk dari koleksi ini.

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


