---
title: "TaskBaseline.CompareTo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskBaseline. Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan"
type: docs
weight: 90
url: /id/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan.

```csharp
public int CompareTo(TaskBaseline other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lain | TaskBaseline | objek Baseline yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

mengembalikan -1 jika instance ini lebih kecil dari objek yang ditentukan, 1 jika instance ini lebih besar dari objek yang ditentukan; jika tidak, mengembalikan 0

## Contoh

Menunjukkan cara memeriksa kesetaraan baseline.

```csharp
var project = new Project();

// membuat TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// menampilkan durasi baseline tugas
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// Kesetaraan baseline diperiksa terhadap angka-angka baseline.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Lihat Juga

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


