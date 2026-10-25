---
title: "Tsk.ActualWorkProtected"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Durasi di mana pekerjaan aktual dilindungi. Pembacaan hanya didukung untuk format XML"
type: docs
weight: 100
url: /id/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

Durasi di mana pekerjaan aktual dilindungi.  Pembacaan hanya didukung untuk format XML.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


