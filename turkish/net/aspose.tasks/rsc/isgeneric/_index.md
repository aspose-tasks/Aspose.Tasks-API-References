---
title: "Rsc.IsGeneric"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın genel (generic) olup olmadığını belirler."
type: docs
weight: 410
url: /tr/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

Bir kaynağın genel olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## Örnekler

Rsc.IsGeneric özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


