---
title: "VbaModuleAttribute.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaModuleAttribute yöntemi. Bu VbaModuleAttribute için bir karma kod değeri döndürür"
type: docs
weight: 40
url: /tr/net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

Bu [`VbaModuleAttribute`](../) için bir karma kod değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

Bu nesne için bir karma kod değeri döndürür.

## Örnekler

Bir VBA modül özniteliğinin karma kodunu nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// VBA modül özniteliklerinin karma kodlarını yazdır
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### Ayrıca Bakınız

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


