---
title: "TreeAlgorithmBase1.PostAlg"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TreeAlgorithmBase. Dipanggil setelah memproses node dalam pohon."
type: docs
weight: 20
url: /id/net/aspose.tasks.util/treealgorithmbase-1/postalg/
---
## TreeAlgorithmBase&lt;T&gt;.PostAlg method

Dipanggil setelah pemrosesan sebuah node pada pohon.

```csharp
public virtual void PostAlg(T el, int level)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Node untuk diproses. |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


