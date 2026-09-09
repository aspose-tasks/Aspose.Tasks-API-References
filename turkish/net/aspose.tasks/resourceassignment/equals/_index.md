---
title: "ResourceAssignment.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment yöntemi. Bu örneğin ResourceAssignment sınıfının belirtilen bir örneğiyle eşit olup olmadığını gösteren bir değer döndürür."
type: docs
weight: 690
url: /tr/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

Bu örneğin [`ResourceAssignment`](../) sınıfının belirtilen bir örneğiyle eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public bool Equals(ResourceAssignment other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | ResourceAssignment | Bu örnek ile karşılaştırılacak [`ResourceAssignment`](../) sınıfının belirtilen örneği. |

### Dönüş Değeri

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## Örnekler

Kaynak ataması eşitliğini nasıl kontrol edeceğini gösterir.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Ayrıca Bakınız

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Bu örnekle karşılaştırılacak nesne. |

### Dönüş Değeri

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## Örnekler

Kaynak ataması eşitliğini nasıl kontrol edeceğini gösterir.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### Ayrıca Bakınız

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


