---
title: "Duration.TimeSpan"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Duration. Mendapatkan instance TimeSpan dari objek Duration ini. Instance TimeSpan dari objek Duration ini"
type: docs
weight: 40
url: /id/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

Mendapatkan instance `TimeSpan` dari objek Duration ini. Instance TimeSpan dari objek Duration ini.

```csharp
public TimeSpan TimeSpan { get; }
```

## Contoh

Menampilkan cara mengonversi durasi menjadi time span.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// ambil durasi tugas
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### Lihat Juga

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


