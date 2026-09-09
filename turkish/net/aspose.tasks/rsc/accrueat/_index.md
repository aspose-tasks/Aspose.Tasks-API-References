---
title: "Rsc.AccrueAt"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Kaynak standart ve fazla mesai maliyetlerinin bir görevin maliyetine ne zaman ve nasıl yansıtılacağını veya tahakkuk ettirileceğini belirler"
type: docs
weight: 10
url: /tr/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

Kaynak standart ve fazla mesai maliyetlerinin bir görevin maliyetine ne zaman ve nasıl yansıtılacağını veya birikeceğini belirler.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## Örnekler

Rsc.AccrueAt özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


