---
title: "VbaModuleAttribute.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaModuleAttribute yöntemi. Bu örneğin belirtilen VbaModuleAttribute nesnesine eşit olup olmadığını gösteren bir değer döndürür"
type: docs
weight: 30
url: /tr/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

Bu örneğin belirtilen [`VbaModuleAttribute`](../) nesnesine eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public bool Equals(VbaModuleAttribute other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | VbaModuleAttribute | Bu örnek ile karşılaştırılacak belirtilen [`VbaModuleAttribute`](../) nesnesi. |

### Dönüş Değeri

Bu örnek belirtilen [`VbaModuleAttribute`](../) nesnesine eşitse true, aksi takdirde false döndürür.

## Örnekler

VBA modül özniteliklerinin eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Ayrıca Bakınız

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Bu örneğin belirtilen [`VbaModuleAttribute`](../) nesnesine eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Bu örnek ile karşılaştırılacak belirtilen [`VbaModuleAttribute`](../) nesnesi. |

### Dönüş Değeri

Bu örnek belirtilen [`VbaModuleAttribute`](../) nesnesine eşitse true, aksi takdirde false döndürür.

## Örnekler

VBA modül özniteliklerinin eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### Ayrıca Bakınız

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


