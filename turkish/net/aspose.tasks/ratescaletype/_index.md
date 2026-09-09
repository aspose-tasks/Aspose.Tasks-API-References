---
title: "RateScaleType enumı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RateScaleType enumı. Oran ölçeği tipini belirtir"
type: docs
weight: 1650
url: /tr/net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

Oran ölçeği türünü belirtir.

```csharp
public enum RateScaleType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `0` | Tanımsız oran ölçeği tipini gösterir. |
| Minute | `1` | Dakika oran ölçeği tipini gösterir. |
| Hour | `2` | Saat oran ölçeği tipini gösterir. |
| Day | `3` | Gün oran ölçeği tipini gösterir. |
| Week | `4` | Hafta oran ölçeği tipini gösterir. |
| Month | `5` | Ay oran ölçeği tipini gösterir. |
| Quarter | `6` | Çeyrek yıl oran ölçeği tipini gösterir. |
| Year | `7` | Yıl oran ölçeği tipini gösterir. |

## Örnekler

Bir malzeme kaynağı ataması için değişken malzeme tüketimini (ör. '10/day' veya '1/week') nasıl ayarlayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// ‘1/week’ malzeme tüketimini ayarlamak istediğimizi varsayalım.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

Bir malzeme kaynağı ataması için değişken malzeme tüketimini (ör. '10/day' veya '1/week') ayarlamak istediğimizde atamanın oran ölçeğiyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// ‘1/week’ malzeme tüketimini ayarlamak istediğimizi varsayalım.
// Saatlik oranı Units özelliğine ayarlamalıyız, bu yüzden 1D'yi haftadaki saat sayısına bölüyoruz.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// Lütfen 24.4 sürümünden itibaren bunun bir yöntem çağrısıyla yapılabileceğini unutmayın:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// Sadece malzeme kaynak atamaları sıfır olmayan bir oran ölçeği değerine sahip olabilir.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


