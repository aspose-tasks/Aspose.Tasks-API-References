---
title: "Rsc.Workgroup"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Tipe workgroup tempat sumber daya termasuk"
type: docs
weight: 700
url: /id/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

Tipe grup kerja yang menjadi tempat sumber daya tersebut berada.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Workgroup.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


