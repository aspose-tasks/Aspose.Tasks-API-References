---
title: "Kelas CheckCircuit"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Util.CheckCircuit. Memeriksa pohon tugas apakah mengandung sirkuit"
type: docs
weight: 2680
url: /id/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

Memeriksa pohon (tugas) apakah mengandung sirkuit.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | Menginisialisasi instance baru dari kelas `CheckCircuit`. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | Periksa apakah objek yang ditentukan sudah diproses. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

## Contoh

Menampilkan cara mendeteksi struktur proyek yang rusak.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// periksa struktur proyek.
// Jika struktur proyek tidak benar, <see cref="TasksException"> akan dilemparkan.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Lihat Juga

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


