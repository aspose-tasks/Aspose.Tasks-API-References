---
title: "Tsk.RegularWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Jumlah total pekerjaan non lembur yang dijadwalkan untuk dilakukan oleh sumber daya"
type: docs
weight: 940
url: /id/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

Total jumlah pekerjaan non-lembur yang dijadwalkan untuk dilakukan oleh sumber daya.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


