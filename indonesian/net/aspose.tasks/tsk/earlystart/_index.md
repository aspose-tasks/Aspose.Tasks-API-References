---
title: "Tsk.EarlyStart"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tanggal paling awal yang memungkinkan sebuah tugas dimulai berdasarkan tanggal mulai awal dari tugas pendahulu dan penerus serta kendala lainnya."
type: docs
weight: 340
url: /id/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

Tanggal terawal yang mungkin dimulai untuk sebuah tugas, berdasarkan tanggal mulai awal dari tugas pendahulu dan penerus serta batasan lainnya.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.EarlyStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


