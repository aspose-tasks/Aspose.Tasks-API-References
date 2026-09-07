---
title: "Tsk.StartText"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Mengembalikan teks awal tugas."
type: docs
weight: 1030
url: /id/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

Mengembalikan teks mulai tugas.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.StartText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


