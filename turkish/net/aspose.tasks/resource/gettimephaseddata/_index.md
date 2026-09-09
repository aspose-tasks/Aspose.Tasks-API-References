---
title: "Resource.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource yöntemi. Belirtilen TimephasedDataType için verilen başlangıç ve bitiş tarihleri arasındaki TimephasedData değerleriyle bu nesne için bir TimephasedDataCollection sınıfı örneği döndürür."
type: docs
weight: 850
url: /tr/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Bu nesne için verilen başlangıç ve bitiş tarihleri arasındaki [`TimephasedData`](../timephaseddata/) değerleriyle belirtilen [`TimephasedDataType`](../../timephaseddatatype/) için [`TimephasedDataCollection`](../../timephaseddatacollection/) sınıfının bir örneğini döndürür.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Zaman aşamalı veri için başlangıç tarihi. |
| bitiş | DateTime | Zaman aşamalı veri için bitiş tarihi. |
| timephasedType | TimephasedDataType | Zaman aşamalı veri türü ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Dönüş Değeri

[`TimephasedData`](../timephaseddata/) listesi.

## Örnekler

İş/maliyet kaynaklarının zaman aşamalı verilerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Kaynağı kimliğiyle al
var resource = project.Resources.GetByUid(1);

// ResourceWork'un zaman aşamalı verilerini yazdır
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// ResourceCost'un zaman aşamalı verilerini yazdır
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Ayrıca Bakınız

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Bu nesne için verilen başlangıç ve bitiş tarihleri arasındaki [`TimephasedData`](../timephaseddata/) değerleriyle [`TimephasedDataCollection`](../../timephaseddatacollection/) döndürür.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Zaman aşamalı veri için başlangıç tarihi. |
| bitiş | DateTime | Zaman aşamalı veri için bitiş tarihi. |

### Dönüş Değeri

[`TimephasedData`](../../timephaseddata/) listesi.

## Örnekler

İş/maliyet kaynaklarının zaman aşamalı verilerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Kaynağı kimliğiyle al
var resource = project.Resources.GetByUid(1);

// ResourceWork'un zaman aşamalı verilerini yazdır
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// ResourceCost'un zaman aşamalı verilerini yazdır
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Ayrıca Bakınız

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


