---
title: "Filter.op_GreaterThanOrEqual"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Filter yöntemi. Bu örneğin belirtilen bir nesneye eşit veya daha büyük olup olmadığını gösteren bir değer döndürür."
type: docs
weight: 140
url: /tr/net/aspose.tasks/filter/op_greaterthanorequal/
---
## Filter GreaterThanOrEqual operator

Bu örneğin belirtilen nesneden büyük veya ona eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public static bool operator >=(Filter a, Filter b)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bir | Filter | İlk filtre. |
| b | Filter | İkinci filtre. |

### Dönüş Değeri

Bu örneğin belirtilen bir nesneye eşit veya daha büyük olup olmadığını gösteren bir değer

## Örnekler

Filtre eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// Filtrelerin eşitliği, filtrenin UID'sine karşı kontrol edilir.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### Ayrıca Bakınız

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


