---
title: "Rsc.CostVariance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Perbedaan antara biaya dasar dan total biaya untuk sebuah sumber daya"
type: docs
weight: 250
url: /id/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

Selisih antara biaya dasar dan total biaya untuk sumber daya.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.CostVariance.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


