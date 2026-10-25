---
title: "Tsk.PreleveledStart"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tanggal mulai tugas sebagaimana sebelum penyeimbangan sumber daya dilakukan"
type: docs
weight: 920
url: /id/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

Tanggal mulai tugas seperti sebelum leveling sumber daya dilakukan.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.PreleveledStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


