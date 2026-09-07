---
title: "Tsk.EarlyFinish"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tanggal terawal yang mungkin selesai sebuah tugas berdasarkan tanggal selesai awal dari tugas pendahulu dan penerus, batasan lain, dan penundaan leveling apa pun"
type: docs
weight: 330
url: /id/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

Tanggal terawal yang mungkin selesai untuk sebuah tugas, berdasarkan tanggal selesai awal dari tugas pendahulu dan penerus, batasan lainnya, serta penundaan leveling apa pun.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.EarlyFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


