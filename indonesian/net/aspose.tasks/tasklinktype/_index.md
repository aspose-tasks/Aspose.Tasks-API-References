---
title: "Enum TaskLinkType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.TaskLinkType. Menentukan jenis ketergantungan tugas"
type: docs
weight: 2440
url: /id/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

Menentukan jenis ketergantungan tugas.

```csharp
public enum TaskLinkType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| FinishToFinish | `0` | Hubungan Selesai-Selesai |
| FinishToStart | `1` | Hubungan Selesai-Mulai |
| StartToFinish | `2` | Hubungan Mulai-Selesai |
| StartToStart | `3` | Hubungan Mulai-Mulai |

## Contoh

Menampilkan cara mendapatkan/mengatur tipe tautan dari tautan tugas.

```csharp
var project = new Project();

// Tambahkan tugas baru
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Tautkan tugas dengan tipe tautan diatur ke Start to Start
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


