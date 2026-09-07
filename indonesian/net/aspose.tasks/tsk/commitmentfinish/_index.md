---
title: "Tsk.CommitmentFinish"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tanggal selesai dari sebuah pengiriman.  Pembacaan hanya didukung untuk format XML."
type: docs
weight: 170
url: /id/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

Tanggal selesai pengiriman.  Pembacaan hanya didukung untuk format XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.CommitmentFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


