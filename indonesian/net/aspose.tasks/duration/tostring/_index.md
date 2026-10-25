---
title: "Duration.ToString"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Duration. Mengembalikan representasi string dari instance ini"
type: docs
weight: 120
url: /id/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

Mengembalikan representasi string dari instance ini.

```csharp
public override string ToString()
```

### Nilai Kembali

representasi string dari instance ini.

## Contoh

Menampilkan cara mengonversi durasi menjadi string.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// ambil durasi tugas
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### Lihat Juga

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


