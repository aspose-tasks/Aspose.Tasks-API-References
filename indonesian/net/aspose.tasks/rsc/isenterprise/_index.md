---
title: "Rsc.IsEnterprise"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Menampilkan apakah sumber daya berasal dari pool sumber daya perusahaan (true) atau pool sumber daya lokal (false)"
type: docs
weight: 400
url: /id/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

Menampilkan apakah sumber daya berasal dari kumpulan sumber daya perusahaan (true) atau kumpulan sumber daya lokal (false).

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.IsEnterprise.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


