---
title: "Rsc.Inactive"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Menentukan apakah sumber daya dinonaktifkan oleh pengguna yang memiliki hak administratif"
type: docs
weight: 360
url: /id/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

Menentukan apakah sumber daya dinonaktifkan oleh pengguna yang memiliki hak administratif.

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Inactive.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


