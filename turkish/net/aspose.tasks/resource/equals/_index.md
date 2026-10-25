---
title: "Resource.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource yöntemi. Bu örneğin Resource sınıfının belirtilen bir örneğiyle eşit olup olmadığını gösteren bir değer döndürür"
type: docs
weight: 820
url: /tr/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

Bu örneğin [`Resource`](../) sınıfının belirtilen bir örneğiyle eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public bool Equals(Resource other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | Resource | Bu örnekle karşılaştırılacak [`Resource`](../) sınıfının belirtilen örneği. |

### Dönüş Değeri

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## Örnekler

Kaynak eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Ayrıca Bakınız

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
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

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## Örnekler

Kaynak eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### Ayrıca Bakınız

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


