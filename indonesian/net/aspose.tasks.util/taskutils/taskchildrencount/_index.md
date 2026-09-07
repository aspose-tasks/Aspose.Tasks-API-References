---
title: "TaskUtils.TaskChildrenCount"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskUtils. Secara rekursif menghitung jumlah tugas anak melalui semua tingkat"
type: docs
weight: 40
url: /id/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

Menghitung secara rekursif jumlah tugas anak dari sebuah tugas melalui semua tingkatan.

```csharp
public static int TaskChildrenCount(Task task)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tugas | Tugas | Tugas yang dihitung oleh anak-anak. |

### Nilai Kembali

Jumlah anak.

## Contoh

Menampilkan cara menggunakan metode &lt;see cref="Aspose.Tasks.Util.TaskUtils.TaskChildrenCount" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// secara rekursif menghitung jumlah tugas anak melalui semua tingkat
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### Lihat Juga

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


