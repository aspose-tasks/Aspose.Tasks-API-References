---
title: "Tsk.StatusManager"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Nama sumber daya perusahaan yang akan menerima pembaruan status untuk tugas saat ini dari sumber daya"
type: docs
weight: 1050
url: /id/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

Nama sumber daya perusahaan yang akan menerima pembaruan status untuk tugas saat ini dari sumber daya.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.StatusManager.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


