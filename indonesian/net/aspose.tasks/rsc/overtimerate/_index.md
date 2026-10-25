---
title: "Rsc.OvertimeRate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Tingkat pembayaran untuk pekerjaan lembur yang dilakukan oleh sumber daya"
type: docs
weight: 510
url: /id/net/aspose.tasks/rsc/overtimerate/
---
## Rsc.OvertimeRate field

Tarif pembayaran untuk pekerjaan lembur yang dilakukan oleh sumber daya.

```csharp
public static readonly Key<decimal, RscKey> OvertimeRate;
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


