---
title: "Tsk.DisplayAsSummary"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah tugas harus ditampilkan sebagai tugas ringkasan. Pembacaan hanya didukung untuk format XML"
type: docs
weight: 280
url: /id/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

Menentukan apakah tugas harus ditampilkan sebagai tugas ringkasan. Pembacaan hanya didukung untuk format XML.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.DisplayAsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


