---
title: "TaskBaseline.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskBaseline. Mengembalikan nilai kode hash untuk instance dari kelas TaskBaseline."
type: docs
weight: 110
url: /id/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

Mengembalikan nilai kode hash untuk instance dari kelas [`TaskBaseline`](../).

```csharp
public override int GetHashCode()
```

### Nilai Kembali

mengembalikan nilai kode hash untuk objek ini.

## Contoh

Menampilkan cara mendapatkan kode hash dari sebuah baseline tugas.

```csharp
var project = new Project();

// membuat TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// menampilkan durasi baseline tugas
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// kode hash dari kalender sama dengan nomor baseline 
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### Lihat Juga

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


