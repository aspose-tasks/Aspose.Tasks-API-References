---
title: "Task.Children"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan koleksi tugas anak dari objek ini. Objek TaskCollection yang mewakili tugas-tugas anak"
type: docs
weight: 190
url: /id/net/aspose.tasks/task/children/
---
## Task.Children property

Mendapatkan koleksi tugas anak dari objek ini. Objek TaskCollection yang mewakili tugas-tugas anak.

```csharp
public TaskCollection Children { get; }
```

## Contoh

Menampilkan cara menggunakan koleksi tugas untuk menambahkan sebuah tugas.

```csharp
var project = new Project();

// Tambahkan tugas, sub tugas, dan simpan proyek
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


