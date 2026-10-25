---
title: "Enum ResourceType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.ResourceType enum. Menentukan tipe sumber daya"
type: docs
weight: 1800
url: /id/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

Menentukan jenis sumber daya.

```csharp
public enum ResourceType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Material | `0` | Menunjukkan tipe sumber daya Material. |
| Work | `1` | Menunjukkan tipe sumber daya Kerja. |
| Cost | `2` | Menunjukkan tipe sumber daya Biaya. |

## Contoh

Menampilkan cara bekerja dengan tipe sumber daya.

```csharp
var project = new Project();

// tambahkan sumber daya kerja
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// tambahkan sumber daya material
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// tambahkan sumber daya material
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// bekerja dengan sumber daya: buat tugas, tugaskan sumber daya, dan sebagainya...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


