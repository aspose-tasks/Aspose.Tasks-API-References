---
title: "Rsc.MaxUnits"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Jumlah unit maksimum yang mewakili kapasitas maksimum dimana sebuah sumber daya tersedia untuk menyelesaikan tugas apa pun selama periode waktu saat ini"
type: docs
weight: 450
url: /id/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

Jumlah maksimum satuan yang mewakili kapasitas maksimum di mana sumber daya tersedia untuk menyelesaikan tugas apa pun selama periode waktu saat ini.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.MaxUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


