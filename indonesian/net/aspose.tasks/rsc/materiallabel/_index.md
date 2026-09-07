---
title: "Rsc.MaterialLabel"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Satuan ukuran untuk sumber daya material"
type: docs
weight: 440
url: /id/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

Satuan ukuran untuk sumber daya material.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.MaterialLabel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


