---
title: "Filter.CompareTo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Filter yöntemi. Bu örneği, Filter sınıfının belirtilen örneğiyle karşılaştırır ve göreceli sıraları hakkında bir gösterge döndürür."
type: docs
weight: 90
url: /tr/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

Bu örneği, [`Filter`](../) sınıfının belirtilen örneğiyle karşılaştırır ve göreceli sıraları hakkında bir gösterge döndürür.

```csharp
public int CompareTo(Filter other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | Filter | bu nesneyle karşılaştırmak için [`Filter`](../) sınıfının belirtilen örneği. |

### Dönüş Değeri

göreceli sıraları hakkında bir gösterge.

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


