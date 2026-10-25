---
title: "Project.RenumberWBSCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Memberi nomor ulang kode WBS semua tugas"
type: docs
weight: 1180
url: /id/net/aspose.tasks/project/renumberwbscode/
---
## RenumberWBSCode() {#renumberwbscode}

Menomori ulang kode WBS semua tugas.

```csharp
public void RenumberWBSCode()
```

## Contoh

Menampilkan cara memberi nomor ulang kode WBS tugas.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

IEnumerable<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// output: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode();

Console.WriteLine("\nWBS codes after: ");

// output: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## RenumberWBSCode(List&lt;int&gt;) {#renumberwbscode_1}

Menomori ulang kode WBS tugas yang telah selesai.

```csharp
public void RenumberWBSCode(List<int> taskIds)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| taskIds | List`1 | Pengidentifikasi tugas untuk memberi nomor ulang kode WBS. |

## Contoh

Menampilkan cara memberi nomor ulang kode WBS tugas yang dipilih.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// output: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// output: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


