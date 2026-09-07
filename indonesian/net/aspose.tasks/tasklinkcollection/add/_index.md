---
title: "TaskLinkCollection.Add"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskLinkCollection. Mengembalikan instance dari FinishStart TaskLink yang telah ditambahkan ke objek TaskLinkCollection."
type: docs
weight: 40
url: /id/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Mengembalikan sebuah instance dari Finish-Start [`TaskLink`](../../tasklink/) yang telah ditambahkan ke objek TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pred | Tugas | Tugas pendahulu. |
| succ | Tugas | Tugas penerus. |

### Nilai Kembali

sebuah instance tautan tugas yang telah ditambahkan ke objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | Jika salah satu tugas masukan bernilai null maka ArgumentNullException akan dilempar. |

## Contoh

Menampilkan cara bekerja dengan koleksi tautan tugas.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// dapatkan tugas
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// tautkan tugas-tugas
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// cetak tautan di antara tugas-tugas
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// sunting tautan dengan akses indeks
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// hapus semua tautan tugas
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Lihat Juga

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

Mengembalikan sebuah instance dari [`TaskLink`](../../tasklink/) yang telah ditambahkan ke objek TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pred | Tugas | Tugas pendahulu. |
| succ | Tugas | Tugas penerus. |
| linkType | TaskLinkType | Tipe tautan [`TaskLinkType`](../../tasklinktype/) |

### Nilai Kembali

sebuah instance tautan tugas yang telah ditambahkan ke objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | Jika salah satu tugas masukan bernilai null maka ArgumentNullException akan dilempar. |

## Contoh

Menampilkan cara bekerja dengan koleksi tautan tugas.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// dapatkan tugas
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// tautkan tugas-tugas
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// cetak tautan di antara tugas-tugas
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// sunting tautan dengan akses indeks
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// hapus semua tautan tugas
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Lihat Juga

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

Mengembalikan sebuah instance dari [`TaskLink`](../../tasklink/) yang telah ditambahkan ke objek TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pred | Tugas | Tugas pendahulu. |
| succ | Tugas | Tugas penerus. |
| linkType | TaskLinkType | Tipe tautan [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Penundaan tautan [`Duration`](../../duration/). |

### Nilai Kembali

sebuah tautan tugas yang telah ditambahkan ke objek ini.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | Jika salah satu tugas masukan bernilai null maka ArgumentNullException akan dilempar. |

## Contoh

Menampilkan cara bekerja dengan koleksi tautan tugas.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// dapatkan tugas
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// tautkan tugas-tugas
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// cetak tautan di antara tugas-tugas
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// sunting tautan dengan akses indeks
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// hapus semua tautan tugas
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Lihat Juga

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Ini adalah implementasi stub dari metode Add milik ICollection, yang hanya melempar NotSupportedException

```csharp
public void Add(TaskLink item)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | TaskLink | Item yang akan ditambahkan. |

### Lihat Juga

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


