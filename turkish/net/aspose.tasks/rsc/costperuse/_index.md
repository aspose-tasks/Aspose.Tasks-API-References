---
title: "Rsc.CostPerUse"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynak her kullanıldığında oluşan maliyet"
type: docs
weight: 240
url: /tr/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

Bir kaynak her kullanıldığında oluşan maliyet.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## Örnekler

Rsc.CostPerUse özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


