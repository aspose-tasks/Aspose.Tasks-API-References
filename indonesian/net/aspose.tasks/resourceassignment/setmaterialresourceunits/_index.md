---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceAssignment. Menetapkan unit untuk penugasan sumber daya material dengan konsumsi material variabel. Konsumsi material variabel berarti bahwa seiring perubahan durasi penugasan, jumlah material yang digunakan berubah secara proporsional."
type: docs
weight: 760
url: /id/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

Mengatur satuan untuk penugasan sumber daya material dengan konsumsi material variabel. Konsumsi material variabel berarti bahwa seiring perubahan durasi penugasan, jumlah material yang digunakan berubah secara proporsional.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| unit | Double | Jumlah unit yang terakumulasi pada periode waktu. |
| rateScaleType | RateScaleType | Periode waktu di mana nilai unit terakumulasi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Jika metode dipanggil untuk penugasan sumber daya non-material. |

## Catatan

Misalnya, untuk mengatur '123/bulan', SetUnitsScaled(123D, RateScaleType.Month) harus dipanggil.

## Contoh

Menampilkan cara mengatur konsumsi material variabel (misalnya '10/hari' atau '1/minggu') untuk penugasan sumber daya material.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Misalkan kita ingin mengatur konsumsi material '1/minggu'.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

### Lihat Juga

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


