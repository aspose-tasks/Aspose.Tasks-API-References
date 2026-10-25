---
title: "Rsc.CanLevel"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynakta kaynak dengelemesinin yapılabilir olup olmadığını belirler"
type: docs
weight: 200
url: /tr/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

Bir kaynak üzerinde kaynak dengelemesinin yapılabilir olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## Örnekler

Rsc.CanLevel özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


