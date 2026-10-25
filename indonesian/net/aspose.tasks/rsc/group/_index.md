---
title: "Rsc.Group"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Grup tempat sumber daya berada"
type: docs
weight: 300
url: /id/net/aspose.tasks/rsc/group/
---
## Rsc.Group field

Grup tempat sumber daya berada.

```csharp
public static readonly Key<string, RscKey> Group;
```

## Contoh

Menampilkan cara mengelola tarif dan grup sumber daya.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Tambahkan resource dan atur beberapa properti
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


