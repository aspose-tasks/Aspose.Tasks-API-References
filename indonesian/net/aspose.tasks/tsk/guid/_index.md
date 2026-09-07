---
title: "Tsk.Guid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Kode identifikasi unik yang dihasilkan untuk sebuah tugas"
type: docs
weight: 460
url: /id/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

Kode identifikasi unik yang dihasilkan untuk sebuah tugas.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.Guid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


