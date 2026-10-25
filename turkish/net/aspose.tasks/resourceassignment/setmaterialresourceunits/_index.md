---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment yöntemi. Değişken malzeme tüketimi olan bir maddi kaynağın ataması için birimleri ayarlar. Değişken malzeme tüketimi, atama süresi değiştikçe kullanılan malzeme miktarının orantılı olarak değişmesi anlamına gelir."
type: docs
weight: 760
url: /tr/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

Değişken malzeme tüketimine sahip bir malzeme kaynağı ataması için birimler ayarlar. Değişken malzeme tüketimi, atama süresi değiştikçe kullanılan malzeme miktarının orantılı olarak değişmesi anlamına gelir.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| birimler | Double | Zaman diliminde biriken birim sayısı. |
| rateScaleType | RateScaleType | Birim değerinin biriktiği zaman dilimi. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Yöntem maddi olmayan kaynak ataması için çağrılırsa. |

## Açıklamalar

Örneğin, '123/ay' ayarlamak için SetUnitsScaled(123D, RateScaleType.Month) çağrılmalıdır.

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

### Ayrıca Bakınız

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


