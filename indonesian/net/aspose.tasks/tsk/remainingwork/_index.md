---
title: "Tsk.RemainingWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Waktu yang masih diperlukan untuk menyelesaikan sebuah tugas atau sekumpulan tugas"
type: docs
weight: 990
url: /id/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

Waktu yang masih diperlukan untuk menyelesaikan sebuah tugas atau sekumpulan tugas.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


