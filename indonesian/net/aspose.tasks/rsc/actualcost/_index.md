---
title: "Rsc.ActualCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Biaya yang timbul untuk pekerjaan yang sudah dilakukan oleh sumber daya pada tugas mereka bersama dengan biaya lain yang tercatat terkait dengan tugas tersebut"
type: docs
weight: 30
url: /id/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

Biaya yang timbul untuk pekerjaan yang sudah dilakukan oleh sumber daya pada tugas mereka, bersama dengan biaya lain yang tercatat terkait tugas tersebut.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.ActualCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


