---
title: "Asn.RateScale"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Satuan waktu untuk tingkat penggunaan penugasan sumber daya material. Mengembalikan 0 jika tidak didefinisikan"
type: docs
weight: 410
url: /id/net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

Unit waktu untuk tingkat penggunaan penugasan sumber daya material. Mengembalikan 0 jika tidak didefinisikan.

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## Contoh

Menampilkan cara bekerja dengan skala tarif penugasan ketika kita ingin mengatur konsumsi material variabel (misalnya '10/hari' atau '1/minggu') untuk penugasan sumber daya material.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Misalkan kita ingin mengatur konsumsi material '1/minggu'.
// Kita harus mengatur tarif per jam ke properti Units, sehingga kita membagi 1D dengan jam per minggu.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// Harap dicatat bahwa mulai versi 24.4, ini dapat dilakukan dengan memanggil 1 metode:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// hanya penugasan sumber daya material yang dapat memiliki nilai skala tarif non-nol.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


