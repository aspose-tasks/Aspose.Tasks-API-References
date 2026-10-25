---
title: "Gridline.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Gridline yöntemi. Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür."
type: docs
weight: 50
url: /tr/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | bu örnek ile karşılaştırılacak belirtilen nesne. |

### Dönüş Değeri

bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak.

## Örnekler

Izgara çizgilerinin eşitliğini nasıl kontrol edeceğini gösterir.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// Izgara çizgilerinin eşitliği, ızgara çizgi tipine karşı kontrol edilir.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// tipi değiştir
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### Ayrıca Bakınız

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


