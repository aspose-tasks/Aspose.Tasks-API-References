---
title: "Tsk.CommitmentType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah sebuah tugas memiliki pengiriman terkait atau ketergantungan pada pengiriman terkait. Pembacaan hanya didukung untuk format XML."
type: docs
weight: 190
url: /id/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

Menentukan apakah sebuah tugas memiliki pengiriman terkait atau ketergantungan pada pengiriman terkait.  Pembacaan hanya didukung untuk format XML.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.CommitmentType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


