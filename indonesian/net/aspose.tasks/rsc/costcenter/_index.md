---
title: "Rsc.CostCenter"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Menunjukkan pusat biaya mana yang harus dibebankan pada biaya yang diakumulasi oleh sumber daya"
type: docs
weight: 230
url: /id/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

Menunjukkan pusat biaya mana yang harus dibebankan pada biaya yang diakumulasi oleh sumber daya.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.CostCenter.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


