---
title: "Tsk.FinishText"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Mengembalikan teks penyelesaian tugas"
type: docs
weight: 410
url: /id/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

Mengembalikan teks selesai tugas.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.FinishText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


