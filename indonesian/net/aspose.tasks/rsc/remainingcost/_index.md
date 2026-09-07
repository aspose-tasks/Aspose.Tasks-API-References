---
title: "Rsc.RemainingCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Biaya terjadwal yang tersisa yang akan dikeluarkan dalam menyelesaikan pekerjaan terjadwal yang tersisa"
type: docs
weight: 580
url: /id/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

Biaya terjadwal yang tersisa yang akan timbul dalam menyelesaikan pekerjaan terjadwal yang tersisa.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.RemainingCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


