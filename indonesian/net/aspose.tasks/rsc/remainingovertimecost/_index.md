---
title: "Rsc.RemainingOvertimeCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Biaya lembur terjadwal yang tersisa untuk sebuah sumber daya"
type: docs
weight: 590
url: /id/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

Biaya lembur terjadwal yang tersisa untuk sebuah sumber daya.

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.RemainingOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


