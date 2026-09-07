---
title: "Tsk.IsMarked"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menunjukkan apakah sebuah tugas ditandai untuk tindakan lebih lanjut atau identifikasi jenis tertentu"
type: docs
weight: 620
url: /id/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

Menampilkan apakah sebuah tugas ditandai untuk tindakan lanjutan atau identifikasi jenis tertentu.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## Catatan

Hanya berlaku untuk format file mpp.

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsMarked.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


