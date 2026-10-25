---
title: "Resource.Get"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Resource. Mengembalikan nilai yang dipetakan ke properti dalam wadah ini"
type: docs
weight: 830
url: /id/net/aspose.tasks/resource/get/
---
## Resource.Get&lt;T&gt; method

Mengembalikan nilai yang dipetakan ke properti ini dalam kontainer ini.

```csharp
public T Get<T>(Key<T, RscKey> key)
```

| Parameter | Deskripsi |
| --- | --- |
| T | tipe nilai yang dipetakan. |
| key | kunci properti yang ditentukan. [`Rsc`](../../rsc/) untuk mendapatkan kunci properti. |

### Nilai Kembali

nilai yang dipetakan ke properti dalam wadah ini.

## Contoh

Menampilkan cara membaca/menulis properti resource umum.

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
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


