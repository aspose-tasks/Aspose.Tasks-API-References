---
title: "Tsk.LevelingDelay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Waktu yang harus ditunda tugas dari tanggal mulai awalnya karena penyeimbangan sumber daya"
type: docs
weight: 770
url: /id/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

Waktu yang harus ditunda dari tanggal mulai awal tugas karena leveling sumber daya.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## Contoh

Menunjukkan cara membaca/menulis properti Tsk.LevelingDelay.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


