---
title: "Project.SelectAllChildTasks"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Mengumpulkan secara rekursif semua tugas anak dari tugas akar"
type: docs
weight: 1230
url: /id/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

Mengumpulkan secara rekursif semua tugas anak dari tugas akar.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Nilai Kembali

Koleksi tugas.

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

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


