---
title: "CheckCircuit.Alg"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode CheckCircuit. Memeriksa apakah objek yang ditentukan sudah diproses"
type: docs
weight: 20
url: /id/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

Periksa apakah objek yang ditentukan sudah diproses.

```csharp
public override void Alg(Task el, int level)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | Tugas | Objek untuk diproses. |
| tingkat | Int32 | Level node pohon. |

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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


