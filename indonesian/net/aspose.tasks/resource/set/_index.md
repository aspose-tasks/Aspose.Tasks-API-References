---
title: "Resource.Set"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Resource. Memetakan properti yang ditentukan ke nilai yang ditentukan dalam wadah ini"
type: docs
weight: 860
url: /id/net/aspose.tasks/resource/set/
---
## Set&lt;T&gt;(Key&lt;T, RscKey&gt;, T) {#set_1}

Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini.

```csharp
public void Set<T>(Key<T, RscKey> key, T val)
```

| Parameter | Deskripsi |
| --- | --- |
| T | tipe nilai yang dipetakan. |
| key | kunci properti yang ditentukan. [`Rsc`](../../rsc/) untuk mendapatkan kunci properti. |
| val | nilai. |

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

---

## Set(Key&lt;DateTime, RscKey&gt;, DateTime) {#set}

Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini.

```csharp
public void Set(Key<DateTime, RscKey> key, DateTime val)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | Key`2 | kunci properti yang ditentukan. [`Rsc`](../../rsc/) untuk mendapatkan kunci properti. |
| val | DateTime | nilai. |

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


