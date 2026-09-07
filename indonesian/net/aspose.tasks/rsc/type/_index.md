---
title: "Rsc.Type"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Tipe sebuah sumber daya"
type: docs
weight: 660
url: /id/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

Tipe sebuah sumber daya.

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Type.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


