---
title: "Rsc.PercentWorkComplete"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Persentase pekerjaan yang selesai di semua tugas"
type: docs
weight: 550
url: /id/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

Persentase pekerjaan yang selesai di semua tugas.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## Contoh

Menampilkan cara membaca persentase pekerjaan selesai sumber daya.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// Tampilkan persentase penyelesaian pekerjaan untuk semua sumber daya
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


