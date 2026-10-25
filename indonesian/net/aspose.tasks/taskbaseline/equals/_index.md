---
title: "TaskBaseline.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskBaseline. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek TaskBaseline yang ditentukan."
type: docs
weight: 100
url: /id/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek `TaskBaseline` yang ditentukan.

```csharp
public bool Equals(TaskBaseline other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lain | TaskBaseline | objek AssignmentBaseline yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

mengembalikan true jika instance ini sama dengan objek TaskBaseline yang ditentukan; jika tidak, false.

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

---

## Equals(object) {#equals_2}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | Objek untuk dibandingkan dengan instance ini. |

### Nilai Kembali

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

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


