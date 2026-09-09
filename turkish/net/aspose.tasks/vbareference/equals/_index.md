---
title: "VbaReference.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaReference yöntemi. Bu örneğin belirtilen VbaReference nesnesine eşit olup olmadığını gösteren bir değer döndürür"
type: docs
weight: 40
url: /tr/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

Bu örneğin belirtilen [`VbaReference`](../) nesnesine eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public bool Equals(VbaReference other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | VbaReference | Bu örnek ile karşılaştırılacak belirtilen [`VbaReference`](../) nesnesi. |

### Dönüş Değeri

Bu örnek belirtilen [`VbaReference`](../) nesnesine eşitse true, aksi takdirde false döndürür.

## Örnekler

VBA referans eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Referansların eşitliği, referansın adına göre kontrol edilir.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Ayrıca Bakınız

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Bu örneğin belirtilen [`VbaReference`](../) nesnesine eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Bu örnek ile karşılaştırılacak belirtilen [`VbaReference`](../) nesnesi. |

### Dönüş Değeri

Bu örnek belirtilen [`VbaReference`](../) nesnesine eşitse true, aksi takdirde false döndürür.

## Örnekler

VBA referans eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Referansların eşitliği, referansın adına göre kontrol edilir.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### Ayrıca Bakınız

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


