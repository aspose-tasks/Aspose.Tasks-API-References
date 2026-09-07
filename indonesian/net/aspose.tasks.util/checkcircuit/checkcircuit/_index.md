---
title: "CheckCircuit.CheckCircuit"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor CheckCircuit. Menginisialisasi sebuah instance baru dari kelas CheckCircuit"
type: docs
weight: 10
url: /id/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

Menginisialisasi sebuah instance baru dari kelas [`CheckCircuit`](../).

```csharp
public CheckCircuit()
```

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

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


