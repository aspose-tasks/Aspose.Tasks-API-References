---
title: "Rsc.PeakUnits"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Unit penugasan maksimum untuk sebuah sumber daya pada satu titik waktu untuk semua tugas yang ditugaskan ke sumber daya tersebut"
type: docs
weight: 540
url: /id/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

Satuan penugasan maksimum untuk sumber daya pada satu titik waktu untuk semua tugas yang ditugaskan kepada sumber daya tersebut.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.PeakUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


