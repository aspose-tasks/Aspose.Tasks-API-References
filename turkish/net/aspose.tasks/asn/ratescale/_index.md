---
title: "Asn.RateScale"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Malzeme kaynağı atamasının kullanım oranı için zaman birimi. Tanımlı değilse 0 döndürür"
type: docs
weight: 410
url: /tr/net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

Malzeme kaynağı atamasının kullanım oranı için zaman birimi. Tanımlı değilse 0 döndürür.

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## Örnekler

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


