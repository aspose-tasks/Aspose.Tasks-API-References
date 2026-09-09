---
title: "Filter.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Filter yöntemi. Bu örneğin belirtilen AssignmentBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür"
type: docs
weight: 100
url: /tr/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

Bu örneğin belirtilen AssignmentBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public bool Equals(Filter other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| diğer | Filter | bu örnekle karşılaştırmak için belirtilen AssignmentBaseline nesnesi. |

### Dönüş Değeri

bu örnek belirtilen AssignmentBaseline nesnesine eşitse true, aksi takdirde false döndürür.

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

---

## Equals(object) {#equals_1}

Bu örneğin belirtilen AssignmentBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | bu örnekle karşılaştırmak için belirtilen AssignmentBaseline nesnesi. |

### Dönüş Değeri

bu örnek belirtilen AssignmentBaseline nesnesine eşitse true, aksi takdirde false döndürür.

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


