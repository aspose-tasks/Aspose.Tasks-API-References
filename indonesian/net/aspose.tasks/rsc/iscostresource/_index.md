---
title: "Rsc.IsCostResource"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Menentukan apakah sebuah sumber daya adalah sumber daya biaya"
type: docs
weight: 390
url: /id/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

Menentukan apakah sumber daya merupakan sumber daya biaya.

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.IsCostResource.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


