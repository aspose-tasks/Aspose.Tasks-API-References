---
title: "Gridline.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Gridline yöntemi. Gridline sınıfının örneği için bir hash kodu değeri döndürür."
type: docs
weight: 60
url: /tr/net/aspose.tasks.visualization/gridline/gethashcode/
---
## Gridline.GetHashCode method

Bir [`Gridline`](../) sınıfının örneği için bir karma kod değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

bu nesne için bir karma kod değeri döndürür.

## Örnekler

Bir gridline'ın karma kodunun nasıl alınacağını gösterir.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// Bir gridline'ın karma kodu iç dahili GUID alanına dayanır. 
Console.WriteLine("Gridline 1 Hash Code: {0}", gridline1.GetHashCode());
Console.WriteLine("Gridline 2 Hash Code: {0}", gridline2.GetHashCode());
```

### Ayrıca Bakınız

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


