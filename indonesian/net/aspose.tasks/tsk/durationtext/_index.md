---
title: "Tsk.DurationText"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Mengembalikan teks durasi tugas"
type: docs
weight: 310
url: /id/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

Mengembalikan teks durasi tugas.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.DurationText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


