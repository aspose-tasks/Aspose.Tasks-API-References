---
title: "VbaReference.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaReference yöntemi. Bu VbaReference için bir karma kod değeri döndürür"
type: docs
weight: 50
url: /tr/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

Bu [`VbaReference`](../) için bir karma kod değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

Bu nesne için bir karma kod değeri döndürür.

## Örnekler

Bir VBA referansının karma kodunu nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Bir referansın karma kodu, iç referansın GUID'inin karma kodudur
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### Ayrıca Bakınız

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


