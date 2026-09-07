---
title: "Prj.ShowProjectSummaryTask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Menentukan apakah menampilkan informasi ringkasan tentang seluruh proyek dalam satu baris dengan bilah tugas ringkasan sendiri di bagian atas tampilan Gantt Chart"
type: docs
weight: 640
url: /id/net/aspose.tasks/prj/showprojectsummarytask/
---
## Prj.ShowProjectSummaryTask field

Menentukan apakah menampilkan informasi ringkasan tentang seluruh proyek dalam satu baris dengan bar tugas ringkasan sendiri di bagian atas tampilan Gantt Chart.

```csharp
public static readonly Key<bool, PrjKey> ShowProjectSummaryTask;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.ShowProjectSummaryTask.

```csharp
var project = new Project();

project.Set(Prj.ShowProjectSummaryTask, true);

Console.WriteLine("Show Project Summary Task: " + project.Get(Prj.ShowProjectSummaryTask));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


