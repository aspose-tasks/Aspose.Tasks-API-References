---
title: "Rsc.CostPerUse"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Biaya yang timbul setiap kali sebuah sumber daya digunakan"
type: docs
weight: 240
url: /id/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

Biaya yang muncul setiap kali sumber daya digunakan.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.CostPerUse.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


