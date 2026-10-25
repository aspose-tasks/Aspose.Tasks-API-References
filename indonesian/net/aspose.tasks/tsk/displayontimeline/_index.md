---
title: "Tsk.DisplayOnTimeline"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah sebuah tugas harus ditampilkan pada tampilan garis waktu"
type: docs
weight: 290
url: /id/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

Menentukan apakah tugas harus ditampilkan pada tampilan garis waktu.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.DisplayOnTimeline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


