---
title: "Tsk.RemainingOvertimeWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Jumlah waktu lembur terjadwal yang tersisa."
type: docs
weight: 980
url: /id/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

Jumlah waktu lembur terjadwal yang tersisa.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


