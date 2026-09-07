---
title: "Tsk.CommitmentStart"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tanggal mulai pengiriman. Pembacaan hanya didukung untuk format XML."
type: docs
weight: 180
url: /id/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

Tanggal mulai pengiriman. Pembacaan hanya didukung untuk format XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.CommitmentStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


