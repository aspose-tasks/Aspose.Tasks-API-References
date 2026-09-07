---
title: "Tsk.PreleveledFinish"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Tanggal selesai tugas sebagaimana sebelum penyeimbangan sumber daya dilakukan"
type: docs
weight: 910
url: /id/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

Tanggal selesai tugas seperti sebelum leveling sumber daya dilakukan.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.PreleveledFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


